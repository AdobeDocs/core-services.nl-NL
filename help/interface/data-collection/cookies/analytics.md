---
description: Meer weten over Adobe Analytics cookies in Adobe Experience Cloud?
solution: Experience Cloud,Analytics,Target
title: Adobe Analytics Cookies
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Adobe Analytics cookies

Adobe Analytics gebruikt cookies om aanvragen van verschillende browsers te onderscheiden en om nuttige informatie op te slaan die een toepassing later kan gebruiken. Zij kunnen ook worden gebruikt om het doorbladeren informatie met klantenverslagen te associëren.

Analytics gebruikt cookies om nieuwe bezoekers anoniem te definiëren, hulp bij het analyseren van gegevens over klikstreams en het bijhouden van historische activiteiten op de website, zoals het reageren op bepaalde campagnes of de duur van de verkoopcyclus.

| Naam cookie | Verlopen | Grootte | Locatie | Beschrijving |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 2 jaar | 45 bytes | Eerste partij | Hiermee slaat u de Experience Cloud-id (ECID) of MID op. Instellen op HTTP-reactie. De MID wordt opgeslagen in de `s_ecid=MCMID` -indeling. Stel deze waarde in nadat de client het AMCV-cookie heeft ingesteld. Het staat blijvende het volgen van eerste-partijidentiteitskaart toe en als verwijzingsID wordt gebruikt als het koekje AMCV verloopt. Dit cookie is niet van toepassing op cookie-implementaties van derden. `SameSite` is ingesteld op Lax. |
| **`s_cc`** | Sessie | 4 bytes | Eerste partij | Hiermee bepaalt u of cookies zijn ingeschakeld. Ingesteld door JavaScript. |
| **`s_sq`** | Sessie | 100-200 bytes | Eerste partij | Wordt gebruikt door Activity Map. Deze bevat informatie over de vorige koppeling waarop de bezoeker heeft geklikt. Ingesteld door JavaScript. |
| **`s_vi`** | 2 jaar | 44 bytes | First-party of `*.omtrdc.net` (derde) | Hiermee worden een unieke bezoeker-id en een unieke tijdstempel opgeslagen. Instellen op HTTP-reactie. Elke bezoekersidentiteitskaart wordt geassocieerd met een bezoekersprofiel op de servers van de Adobe. Bezoekersprofielen worden na 1 jaar inactiviteit verwijderd, ongeacht de vervaldatum van de cookie van de bezoeker. De markering `Secure` wordt ingesteld wanneer `SameSite` &quot;Geen&quot; is en de verbinding HTTPS is. `SameSite` is standaard &quot;Lax&quot; voor cookies van de eerste partij. `SameSite` is &quot;Geen&quot; bij gebruik van cookies van derden, zoals op `omtrdc.net` of `2o7.net` . Stel `SameSite` in op &quot;Geen&quot; wanneer u één CNAME gebruikt om meerdere domeinen of eigenschappen bij te houden. |
| **`s_fid`** | 2 jaar | 33 bytes | Eerste partij | Hiermee slaat u de fallback-unieke bezoeker-id en het tijdstempel op. Wordt ingesteld door JavaScript als de standaard `s_vi` -cookie niet kan worden ingesteld vanwege cookie-beperkingen van derden. Niet gebruikt voor cookie-implementaties van de eerste fabrikant. |
| **`s_ac`** | Meteen | 1 byte | Eerste partij | Helpt het correcte domein te bepalen om de koekjes van het AppMeasurement te plaatsen. Bevat de statische waarde `"1"` . Zodra deze cookie is ingesteld, wordt deze direct verwijderd. |

{style="table-layout:auto"}

## Cookies ingesteld op plug-ins

Sommige implementaties maken gebruik van plug-ins. Dit zijn codefragmenten die aanvullende functionaliteit bieden voor Analytics. Deze plug-ins kunnen cookies instellen die hierboven niet worden vermeld. Zie [ het overzicht van stop-ins van Analytics ](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) voor een lijst van beschikbare stop-ins en welke koekjes die zij plaatsen.
