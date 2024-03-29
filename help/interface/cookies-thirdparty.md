---
description: Leer hoe de ondersteuning voor cookies van derden steeds beperkter is geworden in browsers.
solution: Experience Cloud,Analytics,Target
title: Hoe de veranderingen in derdekoekjessteun klanten beïnvloeden
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 3d12a1b1-c952-4b42-815d-f64b31429cec
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 1%

---

# Hoe de veranderingen in derdekoekjessteun klanten beïnvloeden{#how-changes-to-third-party-cookie-support-impacts-customers}

De ondersteuning voor cookies van derden is in browsers beperkter geworden. Als zodanig heeft Adobe gewerkt aan nieuwe toepassingen die zorgvuldig de vereisten van de klant afstemmen op het recht van de consument op privacy in alle Experience Cloud-toepassingen.

In de volgende lijst ziet u hoe de cookie-ondersteuning van derden de huidige implementaties van Experience Cloud-toepassingen beïnvloedt:

## Adobe Analytics en Adobe Target

* Analytics en Target hebben grotendeels geen invloed omdat dezelfde sitetaken alleen afhankelijk zijn van cookies van de eerste fabrikant. Cookies van andere bedrijven zijn vereist om de gebruikersactiviteit in verschillende domeinen te begrijpen. Voor browsers waar cookies van derden worden geblokkeerd, is het niet mogelijk cookies te traceren tussen domeinen.

## Adobe Experience Manager

* Omdat Adobe Experience Manager volledig binnen het domein van de klant werkt, is er minimale interactie met derdekoekjes en zo minimaal tot geen effect.

## Adobe Social

* Het sociale aspect wordt niet beïnvloed zolang de klant over de nieuwste versie van de code beschikt.

## Adobe Advertising Cloud

* Zoeken:

   * Waar zoeken is geoptimaliseerd op basis van Adobe Analytics-gegevens, heeft de zoekopdracht op dezelfde manier gevolgen als Adobe Analytics.
   * Het verzamelen van conversiegegevens moet onaangetast blijven.

* Weergave:

   * Het vandaag de dag opnieuw op de markt brengen van de vertoning is volledig afhankelijk van het gebruik van derdekoekjes.
   * Weergave is ook sterk afhankelijk van de beschikbaarheid van verschillende advertentienetwerkcookies voor synchronisatie.
   * De totale impact is onbekend. Voor het eerste punt wordt de weergave echter meer beïnvloed dan voor andere services.
   * Adobe werkt intern en met Adobe advertentiepartners samen om de impact op en levering ten volle te evalueren.
