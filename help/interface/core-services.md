---
description: Moderniseer uw Adobe Analytics- en Adobe Target-toepassingen voor services voor meerdere toepassingen. Leer hoe u de services voor Experiencen Cloud gaat gebruiken.
solution: Experience Cloud
title: Toepassingen inschakelen voor services voor meerdere toepassingen
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: 48e79e23-b339-4143-b3b1-969c370efeff
source-git-commit: 55b28d6a16f88955d7259a464bb690ee5985540e
workflow-type: tm+mt
source-wordcount: '2136'
ht-degree: 0%

---

# Implementatie voor Experience Cloud-services inschakelen

Als u onlangs Experience Cloud gebruikend Experience Platform markeringen uitvoerde, bent u reeds opstelling voor de Attributen van de Klant en het publiek van het Experience Cloud. U kunt gebruikers en producten in de Admin Console ook beheren.

Bestaande klanten kunnen hun toepassingsimplementaties moderniseren en Experience Cloud implementeren. Zo kunt u de kenmerken van de klant en de publieksfuncties in Adobe Analytics, Audience Manager en Adobe Target gebruiken. Voor deze implementatie gaat u als volgt te werk:

1. [Deelnemen aan het Experience Cloud en beheerder worden](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementeer de Experience Cloud ID Service](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Kaart rapportsuites aan een organisatie van de Experience Cloud toe](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Uw AppMeasurement Analytics bijwerken](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Adobe Target-implementatie bijwerken](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [De implementatie controleren](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Gebruikers en producten beheren](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Begin met het delen van kenmerk- en publieksgegevens](#section_960C06093623462E8EA247B3E97274A1)

## Deelnemen aan het Experience Cloud en beheerder worden {#section_2423F0BD3DF642658103310EE5EA6154}

Wat u moet doen om zich bij het Experience Cloud aan te sluiten:

1. Zorg ervoor dat u de juiste Adobe Analytics- of Adobe Target-SKU&#39;s hebt.

   * **Adobe Analytics:** Standaard of Premium (niet de verouderde [!DNL SiteCatalyst] SKU).
   * **Adobe Target:** Standaard of Premium.

   >[!NOTE]
   >
   >Voor [!DNL Target], migreren naar at.js van [!DNL mbox.js]. Zie [Upgrade uitvoeren vanaf 0,js 1. x tot at.js 2. x](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/upgrading-from-atjs-1x-to-atjs-20.html).

1. Moderniseer uw implementatie en krijg provisioned een beheerder.

   * Voer de onderstaande stappen uit in [Implementeer de [!UICONTROL Experience Cloud ID Service]](core-services.md#section_3C9F6DF37C654D939625BB4D485E4354).
   * Neem contact op met uw accountmanager en start het inrichtingsproces voor het Experience Cloud.

1. Gebruikers en producten beheren in de [!UICONTROL Admin Console].

### Beheerdersaanmelding

Als u een beheerder bent, kunt u zich aanmelden bij [experience.adobe.com](https://experience.adobe.com).

De **[!UICONTROL Admin Console]** de verbinding is beschikbaar in het menunavigatie van het Experience Cloud.

Zie [Experience Cloud gebruiker en producttoediening](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909) voor meer informatie .

### Gebruikersaanmelding

Als u zich wilt aanmelden bij het Experience Cloud, moeten uw gebruikers:

* Heb een Adobe ID (of Enterprise ID voor uw bedrijf).
* Aanmelden bij [experience.adobe.com](https://experience.adobe.com).
* Behoort tot een toepassingsgroep die is toegewezen aan een ondernemingsgroep.
* Koppel zo nodig hun toepassingsaccounts aan hun Adobe ID (zie hieronder).

### Optioneel: bestaande gebruikersaccounts koppelen.

U hebt waarschijnlijk gebruikers die al lid zijn van toepassingsgroepen, zoals een groep Analytics die u eerder hebt beheerd in [!UICONTROL Analytics] > [!UICONTROL Admin Tools].

Wanneer u deze groepen toewijst aan de ondernemingsgroepen van het Experience Cloud, moeten die gebruikers hun geloofsbrieven van de toepassingsrekening aan hun Adobe ID manueel verbinden.

Zie [Accounts koppelen in de Experience Cloud](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>Nadat ondernemingen en toepassingsgroepen in kaart zijn gebracht, worden de nieuwe gebruikers automatisch verbonden. (De geloofsbrieven van de Oplossing worden automatisch gecreeerd en met hun Adobe ID verbonden.)

In de volgende secties wordt beschreven hoe u uw implementatie kunt moderniseren. Door de implementatie te moderniseren, zijn de kernservices in de Experience Cloud mogelijk.

## Implementeer de [!UICONTROL Experience Cloud ID Service] {#section_3C9F6DF37C654D939625BB4D485E4354}

De [!UICONTROL Experience Cloud ID Service] biedt een gemeenschappelijke id voor integratie tussen toepassingen. Het verstrekt dwars-domeinbezoekersidentificatie en een weg voor dwars apparaat/browser richtend en verpersoonlijking die op de gegevens van CRM wordt gebaseerd die via worden geupload [!UICONTROL Customer Attributes].

De eenvoudigste methode voor het inschakelen van kernservices van Experiencen Cloud is het automatisch activeren voor Analytics en Adobe Target via de [Experience Cloud ID Service-extensie](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html?lang=en) in [!UICONTROL Experience Platform Launch].

Voor de volledige hulp van de Dienst van identiteitskaart van het Experience Cloud (vroeger, bezoekersidentiteitskaart), ga [hier](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=en#intro).

**Niet gebruiken [!UICONTROL Experience Platform tags]?**

Als u dit niet gebruikt [!UICONTROL Experience Platform tags], de id-service handmatig implementeren via de JavaScript-implementatie (`VisitorAPI.js`), als volgt:

| Taak | Beschrijving |
| -----------| ---------- |  
| [Implementeer de Experience Cloud ID Service voor Analytics](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-analytics.html?lang=en) | Adobe raadt ook aan extra [klant-id&#39;s](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=en). Deze id&#39;s zijn gekoppeld aan elke bezoeker en maken huidige en toekomstige functionaliteit in Experience Cloud mogelijk. |
| Bestaande bijwerken `s_code` naar versie H.27.3 of hoger, of naar uw bestaande versie `AppMeasurement.js` naar versie 1.4 of hoger. | Deze bestanden kunnen worden gedownload in het dialoogvenster [Codebeheer](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/code-manager-admin.html?lang=en) in Analytics Admin Tools. (De [JavaScript-implementatie](https://experienceleague.adobe.com/docs/analytics/implementation/js/overview.html?lang=en#js) de gids is beschikbaar als u meer informatie over nodig hebt [!DNL AppMeasurement.js].) |
| De klant-id voor Analytics synchroniseren | Zie [Analyse - de klant-id synchroniseren](core-services.md#section_AD473A6A21C1446498E700363F9A8437) (hieronder). |

{style="table-layout:auto"}

### Analyse en Adobe Target - de klant-id synchroniseren {#section_AD473A6A21C1446498E700363F9A8437}

Als onderdeel van het opzetten van de Experience Cloud-id-service raadt de Adobe aan om analyses en [!DNL Target] die u synchroniseert [klant-id&#39;s](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=en) met het Experience Cloud.

In Adobe Target `mbox3rdpartyid` moet de klant-id ophalen en verzenden naar [!DNL Target]. (Zie [Werken met klantkenmerken](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/working-with-customer-attributes.html?lang=en) in [!DNL Target].)

Wanneer een bezoeker op uw website voor authentiek verklaart, of anders zich identificeert, moet uw implementatie de klantenidentiteitskaart van CRM van die persoon aan de pagina of app blootstellen. Vervolgens kunt u de juiste functieaanroep gebruiken om uw klant-id te synchroniseren met het Experience Cloud. Deze synchronisatie slaat de klant-id van CRM van de bezoeker op in het Experience Cloud en activeert de attributen van die klant voor gebruik in het Experience Cloud.

Bijvoorbeeld, veronderstel dat Bob identiteitskaart van de Klant heeft `52mc210tr42` in uw CRM-systeem. Wanneer het Loodje op uw plaats voor authentiek verklaart, moet u deze identiteitskaart op de pagina blootstellen, en identiteitskaart gebruiken om het op één van twee manieren te synchroniseren:

* Bellen `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` met de service Bezoeker-id. Of,
* Vul de *`Customer ID (52mc210tr42)`* in een prop of eVar.

De klant-id moet op elke [!DNL Analytics] serveraanroep waarvan de klant-id bekend is.

#### Analyse: de klant-id synchroniseren met de backfill-methode voor Data Warehouse

Toen Klantkenmerken voor het eerst beschikbaar kwamen, hadden sommige klanten de Experience Cloud-id-service nog niet geïmplementeerd en konden ze de klantkenmerken niet gemakkelijk gebruiken. Om dit probleem te helpen verlichten, creeerde de Adobe een middel om een backfill van de syncs van identiteitskaart te doen gebruikend de Data Warehouse van Adobe Analytics. Deze functie wordt de Data Warehouse backfill genoemd. De Data Warehouse backfill is nu over het algemeen niet nodig en zal daarom niet langer beschikbaar zijn vanaf oktober 2022.


### Mobiele SDK&#39;s

Zie de *Experience Cloud-id-service* sectie voor syntaxisvoorbeelden over hoe te om extra klant IDs te plaatsen in [Android™](https://experienceleague.adobe.com/docs/mobile-services/android/overview.html?lang=en) en [iOS](https://experienceleague.adobe.com/docs/mobile-services/ios/overview.html?lang=en) Mobiele toepassingen.

### Kenmerken inschakelen voor historische gegevens

Kenmerkgegevens van de klant worden beschikbaar gesteld nadat bezoekers zich hebben aangemeld. Als u de Dienst van identiteitskaart nog niet hebt uitgevoerd, en als u klant IDs in een steun of eVar historisch hebt gevolgd, kunt u om een proces verzoeken dat historische logins naar Experience Cloud verzendt. Met dit proces kunt u direct beginnen met het gebruik van Customer Attributes.

Neem contact op met de klantenservice om historische gegevens in te schakelen.

## Kaart rapportsuites aan een Organisatie van de Experience Cloud {#section_7B08516B01BA421681DF03D0E86CE3BA}

>[!NOTE]
>
>De functie voor het toewijzen van rapportsuite is in november 2020 afgekeurd. Neem contact op met de Klantenondersteuning voor alle vragen.

De diensten van het Experience Cloud (zoals de Dienst van identiteitskaart van het Experience Cloud en [!UICONTROL People service]) zijn gekoppeld aan een organisatie van een Experience Cloud in plaats van aan een afzonderlijke analytische rapportensuite. Om ervoor te zorgen dat deze diensten correct werken, moet elke het rapportreeks van Analytics aan een organisatie van de Experience Cloud in kaart worden gebracht.

## Uw AppMeasurement Analytics bijwerken {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Als u Analytics gebruikt, verifieer dat u op regionale gegevensinzameling (RDC) bent. Als uw gegevensverzamelingsdomein `omtrdc.net`of als uw CNAME is toegewezen aan `omtrdc.net`, u bent op RDC. Zie [Overschakelen naar de RDC](https://experienceleague.adobe.com/docs/analytics/technotes/rdc/regional-data-collection.html?lang=en) voor meer informatie . Als u cookies van de eerste fabrikant gebruikt, raadpleegt u [CNAME en de dienst van identiteitskaart van het Experience Cloud](https://experienceleague.adobe.com/docs/id-service/using/reference/analytics-reference/cname.html?lang=en) voor informatie over gegevensverzameling CNAMEs en dwars-domein het volgen.

U wordt aangeraden de analytische implementatie te moderniseren door uw JavaScript-bibliotheken bij te werken, inclusief de API voor bezoekers. De eenvoudige manier om te verwezenlijken is het toevoegen van een [Adobe Analytics-extensie](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/analytics/overview.html?lang=en) in Experience Platform Data Collection.

## Adobe Target-implementatie bijwerken {#section_C2F4493C7A36406DAE2266B429A4BD24}

* U wordt aangeraden een [Adobe Target-extensie](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/target-v2/overview.html?lang=en) in [!UICONTROL Experience Platform] -tags, zodat de bibliotheek automatisch wordt opgehaald. U kunt ook de [Experience Cloud ID Service-extensie](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html?lang=en) voor Adobe Target (en andere toepassingen) gebruiken [!UICONTROL Experience Platform] -tags. De [!UICONTROL Experience Cloud ID Service] update **is vereist** voor Adobe Target om de People-diensten te gebruiken.
* Als u dit niet gebruikt [!UICONTROL Experience Platform] -tags, [de mbox-bibliotheek bijwerken](https://experienceleague.adobe.com/docs/target/using/implement-target/client-side/implement-target-for-client-side-web.html?lang=en) handmatig.
* Toegang aanvragen om Adobe Analytics te gebruiken als rapportagebron voor [!DNL Adobe Target]. [!DNL Target] en [!DNL Analytics] de gegevens worden gecombineerd op de zelfde servervraag tijdens verwerking zodat de bezoekers tussen de twee toepassingen worden aangesloten. Zie [Analyses voor doelimplementatie](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=en).

  >[!IMPORTANT]
  >
  >Alle klanten van Analytics zijn reeds provisioned voor de kerndiensten zoals de Attributen van de Klant. Als u geen klant van de Analyse bent, contacteer de Zorg van de Klant om te verzoeken om levering.

## De implementatie controleren {#section_E641782A0F4F44AF8C9C91216BE330D5}

Gebruik het volgende proces om ervoor te zorgen dat de Dienst van identiteitskaart van het Experience Cloud correct op uw plaats wordt uitgevoerd.

1. Wis koekjes voor uw plaats zodat kunt u het verzoek aan de Dienst van identiteitskaart van het Experience Cloud zien (het verzoek gebeurt bij het eerste bezoek, dan eens per bezoeker per week).
1. Gebruikend een pakketanalysator of het netwerkpaneel in Webbrowser debugger, zoek een verzoek die naar gaat [!DNL dpm.demdex.net].
1. Controleren of de reactie bevat `d_mid` en een waarde, bijvoorbeeld: `_setMarketingCloudFields({"d_mid":"4235...`
1. Controleer of het verzoek Analytics de `mid` parameter (de Experience Cloud-id). Tijdens de respijtperiode (als deze ingeschakeld is) dient u ook een `aid` parameter (de bezoeker-id van Analytics).

Verwachte reactie met Experience Cloud-id:

![Verwachte reactie met Experience Cloud-id](assets/mac_id_response.png)

Verzoek om analytische afbeelding met Experience Cloud-id (ook wel bekend als `mid` of _bezoeker-id_):

![Afbeeldingsverzoek analyseren met Experience Cloud-id](assets/mid.png)

Experience Cloud-id in de mbox-aanvraag:

![Experience Cloud-id in de mbox-aanvraag](assets/mbox_request.png)

### Wat is de respijtperiode?

Nadat u de Dienst van identiteitskaart van het Experience Cloud opstelt, ontvangen de nieuwe bezoekers niet meer een identiteitskaart van het Experience Cloud van Analytics van uw server van de gegevensinzameling. Als gedeelten van uw site de id-service nog niet hebben geïmplementeerd en bezoekers naar deze secties bladeren, wordt de Experience Cloud-id niet herkend en krijgen bezoekers een oudere Analytics-bezoeker-id toegewezen. Dit kan mogelijke problemen veroorzaken, zoals dubbele bezoeken en onjuiste toewijzing.

Als de ondersteuningssectie van uw site bijvoorbeeld in een aparte CMS wordt beheerd, hebt u mogelijk een ander JavaScript-bestand voor Analytics voor deze sectie. Als u de Experience Cloud-id op uw hoofdsite implementeert voordat u de id-service op de ondersteuningssite implementeert, ontvangen nieuwe bezoekers een oude Analytics-id wanneer ze de ondersteuningssectie bezoeken. Bezoeken die beide secties van de site beslaan, worden als verschillende bezoeken gerapporteerd.

Het implementeren van de Experience Cloud-id-service op sites die meerdere JavaScript-bestanden of andere technologieën (zoals Flash) gebruiken, kan coördinatieproblemen veroorzaken. Deze problemen doen zich voor omdat u de Experience Cloud-id-service voor alle delen van uw site tegelijk moet inschakelen. Door een respijtperiode te configureren, blijven nieuwe bezoekers een Analytics-bezoeker-id ontvangen van de ID-service. Bezoekers kunnen consistent worden geïdentificeerd op gedeelten van uw site die niet zijn bijgewerkt voor gebruik van de bezoekersidentiteitsservice.

## Gebruikers en producten beheren {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Als u weer aan de slag bent, navigeert u naar de [Admin Console](https://adminconsole.adobe.com/), waar u gebruikers en productprofielen kunt beheren.

![Access Admin Console](assets/menu-administration-shell.png)

Zie [Experience Cloud gebruiker en productbeheer](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Klantkenmerken

Gebruikers die worden toegevoegd aan de [!UICONTROL Customer Attributes] groep kan de [!UICONTROL Customer Attributes] menu-item links van Experience Cloud.

## Begin met het delen van kenmerk- en publieksgegevens {#section_960C06093623462E8EA247B3E97274A1}

Profiteer van de volgende functies.

### [!UICONTROL People] > [!UICONTROL Customer Attributes]

Als u gegevens van ondernemingsklanten in een gegevensbestand van het het relatiebeheer van de klant (CRM) vangt, kunt u de gegevens in een gegevensbron van de Attributen van de Klant in het Experience Cloud uploaden. Gebruik de gegevens in [!DNL Adobe Analytics] en [!DNL Adobe Target].

Zie [Klantkenmerken](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

### [!UICONTROL People] > [!UICONTROL Audience Library]

Experience Cloud [!UICONTROL Audiences] Dit is de interface waarmee u een publiek kunt maken, bestaande doelgroepen kunt combineren om een samengesteld publiek te maken en alle gedeelde doelgroepen kunt weergeven.

Zie [Soorten publiek](audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

## Gegevensopslag en openbaarmaking van privacy

Als u het publiek in real time profileren en andere kerndiensten binnen de Adobe gebruikt [!DNL Experience Cloud]Het gebruik van deze services kan van invloed zijn op het datacenter (en het land) waar uw gegevens zich bevinden. Specifiek omdat [!DNL Experience Cloud] gebruikt Audience Manager, gegevens die binnen [!UICONTROL People] De dienst moet binnen de servers van de Audience Manager in de Verenigde Staten verblijven.

Bij het gebruik van services die beschikbaar zijn gesteld via de [!UICONTROL People] de diensten, de soorten gegevens die van andere producten van de Adobe aan publieksbeheer worden verzonden zijn:

* [!DNL Analytics] sleutel/waardeparen (eigenschappen, eVars, lijstvariabelen, enzovoort). Door gebrek, omvatten de logboeklijnen IP adres, met inbegrip van het laatste octet van IP (veronderstellend dat het IP adres niet door IP verduisteringsmontages binnen Adobe werd gewijzigd [!DNL Analytics]).
* Treinen en segmenten waarvoor bezoekers in aanmerking komen op basis van in Audience Manager vastgestelde regels.
* (Optioneel) Een of meer van uw id&#39;s. Afhankelijk van uw implementatie van de id-service, verzendt u mogelijk ook een of meer van uw id&#39;s, zoals CRM-id&#39;s of gehashte e-mailadressen. Als deze gegevens naar de Adobe worden verzonden [!DNL Analytics], wordt het overgedragen naar het management van het publiek van de Adobe. Adobe beveelt aan geen persoonsgegevens aan de Adobe te verstrekken [!DNL Analytics]. Gebruik liever een eenrichtingshash om de gegevens te maskeren voordat deze naar de Adobe worden verzonden.
* Segmenten uit [!DNL Analytics] via de back-end segmentdelingsmogelijkheid
* Het cookie demdex.net wordt ingesteld als cookies van derden niet worden geblokkeerd. De `AMCV_###@AdobeOrg` first-party koekje wordt altijd geplaatst met de Dienst van identiteitskaart van het Experience Cloud.

Al deze gegevenselementen worden aan Adobe Audience Manager geleverd in de vorm van logbestanden. Audience Manager verwerkt en slaat deze gegevens op in de Verenigde Staten. Audience Manager biedt geen optie om deze gegevens buiten de Verenigde Staten op te slaan of te verwerken.

### Cookies en Opt-Outs

Het gebruik van realtime publiekprofilering maakt gebruik van de Audience Manager cookie, in aanvulling op de cookies die worden gebruikt voor [!DNL Analytics] en [!DNL Target].

Als u de juiste opt-outmogelijkheid wilt bieden, moeten bezoekers van uw site de Audience Manager opt-out toevoegen aan uw bestaande opt-outproces.

Zie [Adobe Experience Cloud - Implementatie van Adobe opt-Outs](https://experienceleague.adobe.com/docs/analytics/implementation/js/opt-out.html) voor instructies.

Zie [CNAME&#39;s voor gegevensverzameling en interdomeintracering](https://experienceleague.adobe.com/docs/id-service/using/reference/analytics-reference/cname.html?lang=en) voor het inschakelen van interdomeintracering.
