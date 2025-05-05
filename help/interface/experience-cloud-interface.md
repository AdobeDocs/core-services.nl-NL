---
description: Leer hoe u zich aanmeldt en over de centrale interfacecomponenten in Experience Cloud. Meer informatie over algemene zoekopdrachten, voorkeuren voor uw account en hoe u door de interface kunt navigeren en hulp kunt krijgen.
solution: Experience Cloud
title: Experience Cloud Central UI-componenten
feature: Central Interface Components
topic: Administration
role: Admin, User
level: Beginner, Intermediate, Experienced
source-git-commit: 163dc8ef83fb83a0e51879520bcb3ae697c95144
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 2%

---

# Help bij Experience Cloud-interface

De centrale interfacecomponenten van Experience Cloud omvatten eigenschappen die u toelaten:

* Aanmelden en toegang krijgen tot uw toepassingen en services
* Hulp en zakelijke objecten zoeken met behulp van een algemene zoekopdracht
* Uw accountvoorkeuren beheren (waarschuwingen, meldingen en abonnementen)

## Browserondersteuning in Experience Cloud {#browser}

Voor de beste prestaties is Experience Cloud geoptimaliseerd voor de populairste browsers, inclusief de nieuwste versie, plus de twee vorige versies.

* Chrome
* Edge
* Firefox
* Opera
* Safari

Als uw browser niet in de lijst wordt vermeld, wordt deze mogelijk wel ondersteund, maar wordt u aangeraden een van de vermelde browsers te gebruiken.

>[!NOTE]
>
>Niet alle toepassingen die op het domein van het Experience Cloud worden uitgevoerd steunen alle browsers. Raadpleeg de documentatie bij een bepaalde toepassing als u dit niet zeker weet.

## Taalondersteuning in Experience Cloud {#languages}

Experience Cloud ondersteunt voorkeurstalen voor elke gebruiker, zoals ingesteld in de voorkeuren voor uw gebruikersaccount voor Adobe. Momenteel worden de volgende talen ondersteund:

* Chinees
* Engels
* Frans
* Duits
* Italiaans
* Japans
* Koreaans
* Portugees
* Spaans
* Taiwanees

Hoewel al het toepassingsteam aan globale taalsteun wordt geëngageerd, niet worden alle toepassingen aangeboden in alle hierboven vermelde talen. Als uw primaire taal niet in een toepassing van het Experience Cloud wordt gesteund, kunt u een secundaire taal aan gebrek ook plaatsen aan wanneer toepasselijk. Dit kan in [ de gebruikersvoorkeur van het Experience Cloud worden gedaan ](https://experience.adobe.com/preferences).

## Aanmelden bij Experience Cloud {#signin}

Teken binnen en verifieer dat u in de juiste [ organisatie ](organizations.md) bent.

1. Navigeer aan [ Adobe Experience Cloud ](https://experience.adobe.com).
1. Klik op **[!UICONTROL Sign in with an Adobe ID]**.
1. Controleer of u zich in de juiste organisatie bevindt.

   ![ verifieer uw organisatie ](assets/organizations-menu.png)

   Om te verifiëren dat u aan uw correcte [ organisatie ](organizations.md) het programma hebt geopend, klik **[!UICONTROL Profile]** om organisatienaam te zien. Als u toegang hebt tot meerdere organisaties, kunt u ook de kiezer van **[!UICONTROL Organization]** gebruiken om een andere organisatie weer te geven en naar een andere organisatie te schakelen.

   Als uw organisatie Federated IDs gebruikt, staat het Experience Cloud u toe om binnen met enige aanmelding van uw organisatie te ondertekenen zonder het worden vereist om uw e-mailadres en wachtwoord in te gaan. Voeg `#/sso:@domain` aan Experience Cloud URL (`https://experience.adobe.com`) toe om deze taak te verwezenlijken.

   Stel bijvoorbeeld voor een organisatie met federatieve id&#39;s en het domein `adobecustomer.com` de URL-koppeling in op `https://experience.adobe.com/#/sso:@adobecustomer.com` . U kunt ook rechtstreeks naar een specifieke toepassing gaan door een bladwijzer te maken van deze URL, die bij het toepassingspad wordt gevoegd. (Bijvoorbeeld voor Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics` .)

## Toegang tot Experience Cloud-toepassingen {#navigation}

Nadat u zich hebt aangemeld bij Experience Cloud, hebt u vanuit de uniforme header snel toegang tot al uw toepassingen, services en organisaties.

Klik de toepassingsselecteur ![ menu ](assets/menu-icon.png) om tot de diensten van het Experience Cloud toegang te hebben die u bezit.

![ toepassingen van het Experience Cloud van de Toegang ](assets/platform-core-services.png)

## Zoeken en ondersteunen in Experience Cloud {#search-support}

Het onderzoek van het Experience Cloud staat u toe om naar hulp (documentatie, leerprogramma&#39;s, en cursussen) op [ Experience League ](https://experienceleague.adobe.com/nl#home) te zoeken.

![ Onderzoek en steun in Experience Cloud ](assets/search-menu.png)

Via het menu [!UICONTROL Help] hebt u ook toegang tot:

* **[!UICONTROL Support]:** maak een ondersteuningsticket of neem contact op met de Twitter [!UICONTROL Support] .
* **[!UICONTROL Feedback]:** neem contact op met de Adobe via Feedback en laat ons weten wat u denkt.
* **[!UICONTROL Status]:** ga naar `https://status.adobe.com/experience_cloud` en controleer de operationele status van het product en [!UICONTROL Manage Subscriptions] .
* **[!UICONTROL Developer Connection]:** Navigatie naar `adobe.io` en zoek de documentatie voor ontwikkelaars.

## Accountvoorkeuren {#account-menu}

In het menu met accountvoorkeuren kunt u het volgende doen:

* Geef een donker thema op (niet alle toepassingen ondersteunen dit thema)
* Onderzoek naar [ Organisaties ](organizations.md)
* Afmelden
* Vorm rekening [ voorkeur, berichten, en abonnementen ](#preferences)

### Experience Cloud beheren [!UICONTROL Preferences] {#preferences}

Voorkeuren voor Experiencen Cloud zijn meldingen, abonnementen en waarschuwingen.

* Klik **[!UICONTROL Preferences]** van uw rekeningsmenu ![ voorkeur ](assets/preferences-icon-sm.png) om voorkeur te beheren.

![ beheer Experience Cloud ](assets/preferences-page.png)

Op [!UICONTROL Experience Cloud preferences] kunt u de volgende functies configureren:

| Functie | Beschrijving |
|--- |--- |
| Standaard [ organisatie ](organizations.md) | Selecteer de organisatie die u wilt zien wanneer u het Experience Cloud start. |
| [!UICONTROL Subscriptions] | Selecteer de producten en categorieën waarop u zich wilt abonneren. Meldingen in de pop-up [!UICONTROL Notifications] en in uw e-mail. |
| [!UICONTROL Priority] | Selecteer de categorieën die u als hoge prioriteit wilt worden beschouwd. Deze categorieën zijn duidelijk met een Hoog markering en kunnen voor levering zoals alarm worden gevormd. |
| [!UICONTROL Alerts] | Selecteer de meldingen waarvoor u waarschuwingen wilt weergeven in uw browser. Er worden enkele seconden waarschuwingen weergegeven in de rechterbovenhoek van het venster. |
| E-mails | Geef de frequentie op waarmee je e-mailberichten wilt ontvangen. (Niet verzonden, onmiddellijk, dagelijks of wekelijks.) |

{style="table-layout:auto"}

## Meldingen en aankondigingen {#notifications}

Klik op **[!UICONTROL Notifications]** om meldingen weer te geven die belangrijk zijn voor u, en om aankondigingen van Adobe weer te geven.

![ Meldingen en Mededelingen ](assets/notifications-menu-small.png)

U kunt berichten in [ voorkeur van het Experience Cloud vormen ](#preferences).
