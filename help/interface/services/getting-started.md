---
description: Moderniseer uw Adobe Analytics- en Adobe Target-toepassingen voor services voor meerdere toepassingen. Leer hoe u Experience Cloud-services gaat gebruiken.
solution: Experience Cloud
title: Aan de slag met Experience Cloud Services
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: 48e79e23-b339-4143-b3b1-969c370efeff
source-git-commit: 106ad989c5eef60dabbe4b82deaed9d87b09d795
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 0%

---

# Aan de slag met Experience Cloud-services

Als u onlangs Experience Cloud hebt geïmplementeerd met Experience Platform-tags, bent u al ingesteld op klantkenmerken en Experience Cloud-soorten publiek. U kunt gebruikers en producten ook beheren in de Admin Console.

Bestaande klanten kunnen hun toepassingsimplementaties moderniseren en Experience Cloud implementeren. Zo kunt u de kenmerken van klanten en publiekseigenschappen in Adobe Analytics, Audience Manager en Adobe Target gebruiken.

## Deelnemen aan de Experience Cloud en beheerder worden {#section_2423F0BD3DF642658103310EE5EA6154}

Wat je moet doen om lid te worden van Experience Cloud:

1. Zorg ervoor dat u de juiste Adobe Analytics- of Adobe Target-SKU&#39;s hebt.

   * **Adobe Analytics:** Standaard of Premium (niet erfenis [!DNL SiteCatalyst] SKU).
   * **Adobe Target:** Standaard of Premium.

   >[!NOTE]
   >
   >Voor [!DNL Target] migreert u naar at.js vanuit `mbox.js` . Zie [ Bevorderend van at.js 1. x tot at.js 2. x](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/upgrading-from-atjs-1x-to-atjs-20.html).

1. Gebruikers en producten beheren in de [!UICONTROL Admin Console] .

### Beheerdersaanmelding

Nadat u een beheerder bent, kunt u login bij [ experience.adobe.com ](https://experience.adobe.com).

De koppeling **[!UICONTROL Admin Console]** is beschikbaar in Experience Cloud-menunavigatie.

### Gebruikersaanmelding

Als u zich wilt aanmelden bij Experience Cloud, moeten gebruikers:

* Heb een Adobe ID (of Enterprise ID voor uw bedrijf).
* Teken binnen bij [ experience.adobe.com ](https://experience.adobe.com).
* Behoort tot een toepassingsgroep die is toegewezen aan een ondernemingsgroep.
* Koppel zo nodig hun toepassingsaccounts aan hun Adobe ID (zie hieronder).

### Optioneel: bestaande gebruikersaccounts koppelen.

U hebt waarschijnlijk gebruikers die al lid zijn van toepassingsgroepen, zoals een groep Analytics die u eerder hebt beheerd in [!UICONTROL Analytics] > [!UICONTROL Admin Tools] .

Wanneer u deze groepen toewijst aan Experience Cloud-ondernemingsgroepen, moeten deze gebruikers hun gegevens van de toepassingsaccount handmatig koppelen aan hun Adobe ID.

Zie [ rekeningen van de Verbinding in Experience Cloud ](../administration/organizations.md)

>[!NOTE]
>
>Nadat ondernemingen en toepassingsgroepen in kaart zijn gebracht, worden de nieuwe gebruikers automatisch verbonden. (De geloofsbrieven van de Oplossing worden automatisch gecreeerd en met hun Adobe ID verbonden.)

In de volgende secties wordt beschreven hoe u uw implementatie kunt moderniseren. Door uw implementatie te moderniseren, zijn de basisservices in Experience Cloud mogelijk.

## Implementeer de [!UICONTROL Experience Cloud ID Service] {#section_3C9F6DF37C654D939625BB4D485E4354}

[!UICONTROL Experience Cloud ID Service] biedt een gemeenschappelijke id voor integratie tussen toepassingen. Deze biedt identificatie van gebruikers voor verschillende domeinen en een pad voor apparaatbesturing/browser en personalisatie op basis van CRM-gegevens die zijn geüpload via [!DNL Customer Attributes] .

De eenvoudigste methode om de de kerndiensten van Experience Cloud toe te laten is het automatisch voor Analytics en Adobe Target via de [ uitbreiding van de Dienst van identiteitskaart van Experience Cloud ](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html) in [!UICONTROL Experience Platform Launch] te activeren.

Voor volledige hulp van de Dienst van Experience Cloud ID (vroeger, bezoekersidentiteitskaart), ga [ hier ](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html#intro).

**niet Gebruikend [!UICONTROL Experience Platform tags]?**

Als u [!UICONTROL Experience Platform tags] niet gebruikt, implementeert u de id-service handmatig via JavaScript Deployment (`VisitorAPI.js` ), als volgt:

| Taak | Beschrijving |
| -----------| ---------- |  
| [ voer de Dienst van identiteitskaart van Experience Cloud voor Analytics ](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-analytics.html) uit | Adobe adviseert ook plaatsend extra [ klant IDs ](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html). Deze id&#39;s zijn gekoppeld aan elke bezoeker en maken huidige en toekomstige functionaliteit in Experience Cloud mogelijk. |
| Werk uw bestaande `s_code` bij naar versie H.27.3 of hoger, of uw bestaande `AppMeasurement.js` naar versie 1.4 of hoger. | Deze dossiers zijn beschikbaar voor download in de [ Manager van de Code ](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/code-manager-admin.html) in Hulpmiddelen Admin van Analytics. (De [ gids van de Implementatie van JavaScript ](https://experienceleague.adobe.com/docs/analytics/implementation/js/overview.html#js) is beschikbaar als u meer informatie over `AppMeasurement.js` nodig hebt.) |

{style="table-layout:auto"}

### Analyse en Adobe Target - de klant-id synchroniseren {#section_AD473A6A21C1446498E700363F9A8437}

Als deel van vestiging de Dienst van identiteitskaart van Experience Cloud, adviseert Adobe voor Analytics en [!DNL Target] dat u uw [ klant IDs ](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) met Experience Cloud synchroniseert.

In Adobe Target moet de `mbox3rdpartyid` de klant-id ophalen en verzenden naar [!DNL Target] . (Zie [ Werkend met klantenattributen ](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) in [!DNL Target].)

Wanneer een bezoeker op uw website voor authentiek verklaart, of anders zich identificeert, moet uw implementatie de klantenidentiteitskaart van CRM van die persoon aan de pagina of app blootstellen. Vervolgens kunt u de juiste functieaanroep gebruiken om uw klant-id te synchroniseren met Experience Cloud. Deze synchronisatie slaat de klant-id van CRM van de bezoeker op in Experience Cloud en activeert de kenmerken van die klant voor gebruik in Experience Cloud.

Bijvoorbeeld, veronderstel dat het Loodje identiteitskaart van de Klant `52mc210tr42` in uw systeem van CRM heeft. Wanneer het Loodje op uw plaats voor authentiek verklaart, moet u deze identiteitskaart op de pagina blootstellen, en identiteitskaart gebruiken om het op één van twee manieren te synchroniseren:

* Roep `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` aan met behulp van de service Bezoeker-id. Of,
* Vul de *`Customer ID (52mc210tr42)`* in een proxy of eVar.

De klant-id moet worden ingesteld voor elk [!DNL Analytics] -servergesprek waarvan de klant-id bekend is.

#### Analyse: de klant-id synchroniseren met de Data Warehouse-backfill-methode

Toen klantkenmerken voor het eerst beschikbaar kwamen, hadden sommige klanten de Experience Cloud-id-service nog niet geïmplementeerd en konden ze de klantkenmerken niet gemakkelijk gebruiken. Om dit probleem te verhelpen, heeft Adobe een manier gecreëerd om een back-up van id-syncs te maken met de Adobe Analytics Data Warehouse. Deze functie wordt de Data Warehouse-backfill genoemd. De Data Warehouse-backfill is nu over het algemeen niet meer nodig en zal daarom niet langer beschikbaar zijn vanaf oktober 2022.


### Mobiele SDK&#39;s

Zie de *sectie van de Dienst van identiteitskaart van Experience Cloud* voor syntaxisvoorbeelden over hoe te om extra klant IDs in [ Android™ ](https://experienceleague.adobe.com/docs/mobile-services/android/overview.html) en [ iOS ](https://experienceleague.adobe.com/docs/mobile-services/ios/overview.html) Mobiele toepassingen te plaatsen.

### Kenmerken voor historische gegevens inschakelen

Kenmerkgegevens van de klant worden beschikbaar gesteld nadat bezoekers zich hebben aangemeld. Als u de Dienst van identiteitskaart nog niet hebt uitgevoerd, en als u klant IDs in een prep of eVar historisch hebt gevolgd, kunt u om een proces verzoeken dat historische logins naar Experience Cloud verzendt. Met dit proces kunt u direct beginnen met het gebruik van klantkenmerken.

Neem contact op met de klantenservice om historische gegevens in te schakelen.

## Rapportsuites toewijzen aan een Experience Cloud-organisatie {#section_7B08516B01BA421681DF03D0E86CE3BA}

>[!NOTE]
>
>De functie voor het toewijzen van rapportsuite is in november 2020 afgekeurd. Neem contact op met de Klantenondersteuning voor alle vragen.

Experience Cloud-services (zoals Experience Cloud ID Service) zijn gekoppeld aan een Experience Cloud-organisatie in plaats van aan een afzonderlijke Analytics-rapportensuite. Om ervoor te zorgen dat deze services correct werken, moet elke serie Analytics-rapporten worden toegewezen aan een Experience Cloud-organisatie.

## De AppMeasurement-code voor Analytics bijwerken {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Als u eerste-partijkoekjes gebruikt, verwijs naar [ NAAM en de Dienst van identiteitskaart van Experience Cloud ](https://experienceleague.adobe.com/docs/id-service/using/reference/analytics-reference/cname.html) voor informatie over gegevensinzameling CNAMEs en dwars-domein het volgen.

U wordt aangeraden de implementatie van Analytics te moderniseren door uw JavaScript-bibliotheken bij te werken, inclusief de API voor bezoekers. De eenvoudige manier te verwezenlijken is een [ uitbreiding van Adobe Analytics ](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/analytics/overview.html) in de Inzameling van Gegevens van Experience Platform toe te voegen.

## Adobe Target-implementatie bijwerken {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Men adviseert dat u een [ uitbreiding van Adobe Target ](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/target-v2/overview.html) in [!UICONTROL Experience Platform] markeringen toevoegt, zodat uw bibliotheekherwinning automatisch is. U kunt opstelling ook de [ uitbreiding van de Dienst van identiteitskaart van Experience Cloud ](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html) voor Adobe Target (en andere toepassingen) gebruiken [!UICONTROL Experience Platform] markeringen. De [!UICONTROL Experience Cloud ID Service] update **wordt vereist** voor Adobe Target om de diensten van Mensen te gebruiken.
* Als u [!UICONTROL Experience Platform] markeringen niet gebruikt, [ werk manueel uw mbox bibliotheek ](https://experienceleague.adobe.com/docs/target/using/implement-target/client-side/implement-target-for-client-side-web.html) bij.
* Toegang aanvragen om Adobe Analytics als rapportagebron voor [!DNL Adobe Target] te gebruiken. [!DNL Target] - en [!DNL Analytics] -gegevens worden tijdens de verwerking gecombineerd op dezelfde serveraanroep, zodat bezoekers verbinding hebben tussen de twee toepassingen. Zie [ Analytics voor de Implementatie van het Doel ](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html).

  >[!IMPORTANT]
  >
  >Alle klanten van Analytics zijn reeds provisioned voor de kerndiensten zoals klantenattributen. Als u geen klant van de Analyse bent, contacteer de Zorg van de Klant om te verzoeken om levering.

## De implementatie controleren {#section_E641782A0F4F44AF8C9C91216BE330D5}

Ga als volgt te werk om ervoor te zorgen dat Experience Cloud ID Service correct op uw site wordt geïmplementeerd.

1. Cookies wissen voor uw site zodat u de aanvraag voor de Experience Cloud-id-service kunt zien (de aanvraag vindt plaats bij het eerste bezoek en vervolgens eenmaal per bezoeker per week).
1. Gebruikend een pakketanalysator of het netwerkpaneel in Webbrowser debugger, zoek een verzoek die naar [!DNL dpm.demdex.net] gaat.
1. Controleer of het antwoord `d_mid` en een waarde bevat, bijvoorbeeld: `_setMarketingCloudFields({"d_mid":"4235...`
1. Controleer of het verzoek Analytics de parameter `mid` bevat (de Experience Cloud-id). Tijdens de respijtperiode (als deze is ingeschakeld) wordt ook een parameter `aid` (de bezoeker-id van Analytics) weergegeven.

Verwachte reactie met de Experience Cloud-id:

![ Verwachte reactie die identiteitskaart van Experience Cloud ](../assets/mac_id_response.png) bevatten

Het beeldverzoek van de analyse die identiteitskaart van Experience Cloud (ook als `mid` of _bezoekersidentiteitskaart_ wordt bekend) bevat:

![ het beeldverzoek van Analytics die identiteitskaart van Experience Cloud ](../assets/mid.png) bevatten

Experience Cloud-id in de mbox-aanvraag:

![ identiteitskaart van Experience Cloud in het mbox verzoek ](../assets/mbox_request.png)

### Wat is de respijtperiode?

Nadat u de Experience Cloud ID Service hebt geïmplementeerd, ontvangen nieuwe bezoekers geen Analytics Experience Cloud ID meer van uw gegevensverzamelingsserver. Als gedeelten van uw site de ID-service nog niet hebben geïmplementeerd en bezoekers naar deze secties bladeren, wordt de Experience Cloud-id niet herkend en krijgen bezoekers een oudere Analytics-bezoeker-id toegewezen. Dit kan mogelijke problemen veroorzaken, zoals dubbele bezoeken en onjuiste toewijzing.

Als de ondersteuningssectie van uw site bijvoorbeeld in een aparte CMS wordt beheerd, hebt u mogelijk een ander Analytics JavaScript-bestand voor deze sectie. Als u de Experience Cloud-id op uw hoofdsite implementeert voordat u de id-service op de ondersteuningssite implementeert, ontvangen nieuwe bezoekers een oude Analytics-id wanneer ze de ondersteuningssectie bezoeken. Bezoeken die beide secties van de site beslaan, worden als verschillende bezoeken gerapporteerd.

Het implementeren van de Experience Cloud-id-service op sites die meerdere JavaScript-bestanden of andere technologieën (zoals Flash) gebruiken, kan coördinatieproblemen veroorzaken. Deze problemen doen zich voor omdat u de Experience Cloud-id-service voor alle delen van uw site tegelijk moet inschakelen. Door een respijtperiode te configureren, blijven nieuwe bezoekers een Analytics-bezoeker-id ontvangen van de ID-service. Bezoekers kunnen consistent worden geïdentificeerd op gedeelten van uw site die niet zijn bijgewerkt voor gebruik van de bezoekersidentiteitsservice.

## Gebruikers en producten beheren {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Zodra u in gebruik bent, navigeer aan [ Admin Console ](https://adminconsole.adobe.com/), waar u gebruikers en productprofielen kunt beheren.

![ Toegang Admin Console ](../assets/menu-administration-shell.png)

### Klantkenmerken

Gebruikers die aan de groep [!DNL Customer Attributes] zijn toegevoegd, kunnen de menuoptie [!DNL Customer Attributes] aan de linkerkant van Experience Cloud zien.

## Begin met het delen van kenmerk- en publieksgegevens {#section_960C06093623462E8EA247B3E97274A1}

Profiteer van de volgende functies.

### [!UICONTROL Customer attributes]

Als u gegevens van ondernemingsklanten in een gegevensbestand van het het relatiebeheer van de klant (CRM) vangt, kunt u de gegevens in een gegevensbron van de klantenattributen in Experience Cloud uploaden. Gebruik na het uploaden de gegevens in [!DNL Adobe Analytics] en [!DNL Adobe Target] .

Zie [ klantenattributen ](customer-attributes/attributes.md) voor meer informatie.

### [!UICONTROL People] > [!UICONTROL Audience Library]

Experience Cloud [!UICONTROL Audiences] is de interface waarmee u een publiek kunt maken, bestaande doelgroepen kunt combineren om een samengesteld publiek te maken en alle gedeelde doelgroepen kunt bekijken.

Zie [ Soorten publiek ](audiences/overview.md) voor meer informatie.

## Gegevensopslag en openbaarmaking van privacy

Als u realtime profielen voor het publiek en andere kernservices binnen de Adobe [!DNL Experience Cloud] gebruikt, kan het gebruik van deze services van invloed zijn op het datacenter (en het land) waar uw gegevens zich bevinden. Met name omdat [!DNL Experience Cloud] Audience Manager gebruikt, moeten gegevens die in de [!UICONTROL People] -service worden gebruikt, zich in Audience Manager-servers in de Verenigde Staten bevinden.

Wanneer u services gebruikt die via de [!UICONTROL People] -service beschikbaar zijn gesteld, worden de volgende typen gegevens verzonden van andere Adobe-producten naar het beheer van de doelgroep:

* [!DNL Analytics] sleutel/waardeparen (eigenschappen, eVars, lijstvariabelen, enzovoort). Door gebrek, omvatten de logboeklijnen IP adres, met inbegrip van het laatste octet van IP (veronderstellend dat het IP adres niet door IP verduisteringsmontages binnen Adobe [!DNL Analytics] werd gewijzigd).
* Treinen en segmenten waarvoor bezoekers in aanmerking komen op basis van in Audience Manager vastgestelde regels.
* (Optioneel) Een of meer van uw id&#39;s. Afhankelijk van uw implementatie van de id-service, verzendt u mogelijk ook een of meer van uw id&#39;s, zoals CRM-id&#39;s of gehashte e-mailadressen. Als deze gegevens naar Adobe [!DNL Analytics] worden verzonden, worden ze overgebracht naar het publieksbeheer van Adobe. Adobe raadt aan geen persoonlijke gegevens aan te leveren aan Adobe [!DNL Analytics] . Gebruik liever een eenrichtingshash om de gegevens te maskeren voordat deze naar Adobe worden verzonden.
* Segmenten van oorsprong uit [!DNL Analytics] via de back-end segmentdelingsmogelijkheid
* Het cookie demdex.net wordt ingesteld als cookies van derden niet worden geblokkeerd. Het cookie van de eerste gebruiker van `AMCV_###@AdobeOrg` wordt altijd ingesteld met de Experience Cloud ID Service.

Al deze gegevenselementen worden aan Adobe Audience Manager geleverd in de vorm van logbestanden. Audience Manager verwerkt en slaat deze gegevens op in de Verenigde Staten. Audience Manager biedt geen optie om deze gegevens buiten de Verenigde Staten op te slaan of te verwerken.
