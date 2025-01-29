---
description: Leer over centrale interfacecomponenten voor Experience Cloud. Krijg hulp op gebruiker en productbeleid in de Admin Console, laat toepassingen voor de diensten van het Experience Cloud toe. Hulp bij Audience Library, Customer Attributes, Experience Cloud Assets en meer.
title: Interface-documentatie Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 163dc8ef83fb83a0e51879520bcb3ae697c95144
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 10%

---

# Overzicht van de centrale interface van Experience Cloud

[ Experience Cloud ](https://experience.adobe.com) is de geïntegreerde familie van de Adobe van digitale marketing toepassingen, producten, en de diensten. Via de intuïtieve interface hebt u snel toegang tot uw cloudtoepassingen, productfuncties en services.

![ Experience Cloud ](assets/landing.png)

Vanuit de koptekst van Experience Cloud kunt u:

* Heb toegang tot al uw toepassingen en de diensten van het Experience Cloud
* Zoek in het menu Help naar productdocumentatie, zelfstudies en communityartikelen. Resultaten weergeven in Experience League.
* Zakelijke objecten zoeken op algemene wijze met een algemene zoekopdracht (alleen voor gebruikers van Experience Platforms) in het veld Zoeken.
* Beheer uw rekening [ voorkeur ](features/account-preferences.md) (alarm, berichten, en abonnementen)

## Aanmelden bij Experience Cloud {#signin}

Teken binnen en verifieer dat u in de juiste [ organisatie ](administration/organizations.md) bent.

1. Navigeer aan [ Adobe Experience Cloud ](https://experience.adobe.com).
1. Typ uw Adobe-e-mailadres en klik op **[!UICONTROL Continue]** .
1. Selecteer een account.
1. Typ uw wachtwoord.
1. Controleer of u zich in de juiste organisatie bevindt.

   ![ verifieer dat u in de juiste organisatie ](assets/organizations-menu.png) bent

   **verifieer uw organisatie**

   De [ organisatie ](administration/organizations.md) wordt getoond in de interfacekop.

   Als uw organisatie Federated IDs gebruikt, staat het Experience Cloud u toe om binnen met enige aanmelding van uw organisatie te ondertekenen zonder het worden vereist om uw e-mailadres en wachtwoord in te gaan. Voeg `#/sso:@domain` aan Experience Cloud URL (`https://experience.adobe.com`) toe om deze taak te verwezenlijken.

   Stel bijvoorbeeld voor een organisatie met federatieve id&#39;s en het domein `adobecustomer.com` de URL-koppeling in op `https://experience.adobe.com/#/sso:@adobecustomer.com` . U kunt ook rechtstreeks naar een specifieke toepassing gaan door een bladwijzer te maken van deze URL, die bij het toepassingspad wordt gevoegd. (Bijvoorbeeld voor Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics` .)

## Toegang tot Experience Cloud-toepassingen {#navigation}

Nadat u zich hebt aangemeld bij Experience Cloud, hebt u vanuit de uniforme header snel toegang tot al uw toepassingen, services en organisaties.

Om tot de toepassingen en de diensten van het Experience Cloud toegang te hebben die voor u binnen uw organisatie worden voorzien, ga het menu van de toepassingsselecteur ![ ](assets/menu-icon.png).

![ toepassingen van het Experience Cloud van de Toegang ](assets/platform-core-services.png)

## Hulp en ondersteuning {#support}

Het leren van de toegang en hulp die **[!UICONTROL Help center]** (![ activa ](assets/help-icon.png)) gebruiken in de kopbal, met inbegrip van hulpinhoud (documentatie, leerprogramma&#39;s, en cursussen) op [ Experience League ](https://experienceleague.adobe.com/#home), evenals extra middelen voor individuele toepassingen. U kunt ook feedback voor onbepaalde tijd verzenden en geprioriteerde ondersteuningstickets maken.

![ krijg hulp en steun ](assets/search-menu.png)

Via het menu [!UICONTROL Help] hebt u ook toegang tot:

* **[!UICONTROL Support]:** maak een ondersteuningsticket of neem contact op met de Twitter [!UICONTROL Support] .
* **[!UICONTROL Feedback]:** Deel feedback over uw ervaringen met Experiencen Cloud. Je feedback wordt gebruikt om de producten en services van de Adobe te verbeteren.
* **[!UICONTROL Status]:** ga naar `https://status.adobe.com/experience_cloud` en controleer de operationele status van het product en [!UICONTROL Manage Subscriptions] .
* **[!UICONTROL Developer Connection]:** Navigatie naar `adobe.io` en zoek de documentatie voor ontwikkelaars.

## Uw gebruikersprofiel beheren

In het menu [!UICONTROL Profile] kunt u:

* Geef een donker thema op (niet alle toepassingen ondersteunen dit thema)
* Beheer Experience Cloud [ Voorkeur ](features/account-preferences.md)
* Selecteer of onderzoek naar een [ Organisatie ](administration/organizations.md)
* Weergeven [!UICONTROL Legal Notices]
* Afmelden
* Accountvoorkeuren, meldingen en abonnementen configureren

## Meldingen en aankondigingen in producten weergeven {#notifications}

Klik op het belpictogram om meldingen en aankondigingen weer te geven. Aankondigingen kunnen relevante en actiefuncties zijn, zoals productreleases, onderhoudsmeldingen, gedeelde items en goedkeuringsaanvragen.

![ Meldingen en Mededelingen ](assets/notifications-menu-small.png)

Om berichten en alarm te beheren, zie [ voorkeur en berichten van de Rekening ](features/account-preferences.md)


## Nieuwe functies

Leer over de recentste verhogingen aan de centrale interfacecomponenten van het Experience Cloud.

>[!BEGINTABS]

>[!TAB  integratie van de Slack met Experience Cloud ]

U kunt uw accountvoorkeuren zo configureren dat meldingen van Experiencen Cloud naar een [!DNL Slack] -kanaal worden verzonden.

[!BADGE Bèta]{type=Informative url="https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#notifications" tooltip="Meer informatie over Slack"}


>[!TAB  Nieuw Gebruikersinterface van het Web van de Campagne ]

Ervaar de nieuwe Adobe Campaign-gebruikersinterface. modernere, intuïtievere en dynamischer!

[![afbeelding](assets/do-not-localize/learn-more-button.svg)](start/campaign-ui.md#ac-web-ui)


>[!TAB  het kanaal van de duw aanstaande veranderingen ]

In 2024 komt er een versie met enkele belangrijke wijzigingen voor de service FCM (Android Firebase Cloud Messaging). Deze kunnen van invloed zijn op uw Adobe Campaign-implementatie. De configuratie van uw lidmaatschapsservices voor Android-pushberichten moet mogelijk worden bijgewerkt om deze wijziging te ondersteunen. U kunt het nu al controleren en actie ondernemen.

[![afbeelding](assets/do-not-localize/learn-more-button.svg)](../technotes/upgrades/push-technote.md)



>[!ENDTABS]

## Starten met de basisprincipes

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
    <a href="start/whats-new.md"><img src="assets/do-not-localize/start-capabilities.png"></a>
    <div><strong> Zeer belangrijke mogelijkheden </strong><br/> ontdekken de zeer belangrijke mogelijkheden van Adobe Campaign v8 voor het beheer van de dwars-kanaalcampagne.</div>
    </td>
    <td>
    <a href="start/connect.md"><img src="assets/do-not-localize/start-connect.jpeg"></a>
    <div><strong> verbind met Campagne v8 </strong><br/> Leer hoe te met Adobe Campaign v8 te verbinden en uw reis van het campagnebeheer te kickstart door de cliëntconsole te installeren en te vormen.</div><br/>
    </td>
    <td>
    <a href="start/create-message.md"><img src="assets/do-not-localize/start-send.jpeg"></a>
    <div><strong> verzendt berichten </strong><br/> leren hoe te om berichten over diverse kanalen zoals e-mail, SMS, duw berichten onder anderen te verzenden.
    </div></td>
    <td>
    <a href="audiences/create-profiles.md"><img src="assets/do-not-localize/start-profiles.png"></a>
    <div><strong> de Profielen van de Invoer </strong><br/> ontdekken profielverwezenlijking in het gegevensbestand van Adobe Campaign v8 met gemak. Voeg profielen handmatig of via importeren toe, verfijn klantgegevens en pas campagnes moeiteloos aan.</div>
    </td>
  </tr>
  <tr style="border: 0;">
    <td align="center"><a href="start/whats-new.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/connect.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/create-message.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="audiences/create-profiles.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    </tr>
</table>

## De documentatie verkennen

<table style="table-layout:auto">
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon-start.svg" width="35px">
    <br/>
      <strong> krijgen begonnen </strong><br/> <a href="start/campaign-ui.md"> gebruikersinterface </a> - <a href="start/ac-components.md"> Componenten &amp; processen </a> - <a href="start/v7-to-v8.md"> van Klassieke v7 aan v8 </a> - <a href="start/campaign-faq.md"> Veelgestelde vragen </a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-experience.svg" width="35px">
    <br/>
      <strong> de ervaring van de Klant </strong><br/> <a href="../automation/workflow/about-workflows.md" target="_blank"> Automatiseer met werkschema's </a> - <a href="../automation/campaigns/set-up-campaigns.md" target="_blank"> Organiseren van de Campagne </a> - <a href="interaction/interaction.md"> Beslissingsbeheer </a> - <a href="send/personalize.md"> Personalization </a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-send.svg" width="35px">
    <br/>
      <strong> verzend berichten </strong><br/> <a href="start/create-message.md"> begonnen worden </a> - <a href="send/preview-and-proof.md"> Voorproef &amp; proef </a> - <a href="send/predictive.md"> Send-time optimalisering </a> - <a href="reporting/gs-reporting.md"> Rapporterend &amp; Analytics </a>
    </td>
  </tr>
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon_profile-audience.svg" width="35px">
    <br/>
      <strong> Profielen &amp; publiek </strong><br/> <a href="audiences/create-profiles.md"> voegt profielen </a> toe - <a href="audiences/create-audiences.md"> leidt publiek </a> - <a href="start/subscriptions.md"> beheert abonnementen </a> - <a href="start/privacy.md"> Privacy </a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-configure.svg" width="35px">
    <br/>
      <strong> Architectuur &amp; configuratie </strong><br/> <a href="architecture/architecture.md"> Architectuur </a> - <a href="start/implement.md"> de implementatie van de Campagne v8 </a> - <a href="connect/integration.md"> verbindt met andere oplossingen </a> - <a href="start/gs-permissions.md"> Gebruikers &amp; toestemmingen </a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-dev.svg" width="35px">
    <br/>
      <strong> middelen van de Ontwikkelaar </strong><br/> <a href="dev/datamodel.md"> Campagne v8 gegevensmodel </a> - <a href="dev/schemas.md"> Schema's </a> - <a href="dev/api.md"> APIs </a>
    </td>
  </tr>
</table>

## Aanvullende bronnen

[ Adobe Campaign v8 Beschrijving van het Product ](https://helpx.adobe.com/nl/legal/product-descriptions/adobe-campaign-managed-cloud-services.html) {target="_blank"} - [ de gebruikersinterfacedocumentatie van het Web van Adobe Campaign ](https://experienceleague.adobe.com/docs/campaign-web/v8/campaign-web-home.html) {target="_blank"} - [ Tutorials ](https://experienceleague.adobe.com/docs/campaign-learn/tutorials/overview.html) {target="_blank"} - [[!DNL Adobe Campaign]  automatiseringsgids ](https://experienceleague.adobe.com/docs/campaign/automation/home.html) {target="_blank"} - [ Controlebord voor Campagne v8 ](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/key-features.html?lang=nl) {target="_blank"}

