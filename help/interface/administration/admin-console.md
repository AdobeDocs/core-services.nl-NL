---
title: Licentiebeheer voor gebruikers en producten
description: Gebruikers en productlicenties beheren in Admin Console for Experience Cloud-toepassingen.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: 9932f21e4aa4d4a5bf08d7f1617b4c25d4fb14bb
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 2%

---

# Gebruikersbeheer en productlicenties

Deze pagina bevat specifiek informatie voor Experience Cloud-beheerders, met koppelingen naar algemene documentatie over gebruikers en productbeheer.

Voor algemene hulp van het identiteitsbeheer toepasselijk op alle toepassingen van Adobe, zie de [ gids van de Onderneming en van teamadmin ](https://helpx.adobe.com/nl/enterprise/admin-guide.html).

In de volgende secties vindt u koppelingen naar bronnen in de Help van Admin Console.

## Administratieve taken in Admin Console

De Admin Console biedt drie primaire administratieve taken, elk met specifieke niveaus van toegang en verantwoordelijkheid:

**beheerder van het Systeem:** Volledige toegang - beheert alle aspecten van de console.

Belangrijkste verantwoordelijkheden:

* Gebruikers toevoegen, verwijderen en beheren.
* Productlicenties toewijzen en intrekken.
* Identiteitsinstellingen en verificatie configureren.
* Factureringsgegevens weergeven en beheren.
* Stel aanvullende beheerders en gedelegeerde rollen in.

  **Best voor:** de beheerders of het team van IT leiden die het milieu van Adobe van de volledige organisatie controleren.

**de beheerder van het Product:** product-specifiek beheer - controleert toegang en toestemmingen voor specifieke producten van Adobe.

Belangrijkste verantwoordelijkheden:

* Licenties toewijzen en beheren voor een specifiek product.
* Productprofielen maken en beheren.
* Voeg of verwijder gebruikers binnen toegewezen producten toe.

  **Best voor:** Teams/gebruikers die specifieke software zoals Marketo Engage of Adobe Creative Cloud beheren.

**de profielbeheerder van het Product:** Korrelig rolbeheer - concentreert zich op het beheren van gebruikersgroepen en toestemmingen binnen een product.

* Belangrijkste verantwoordelijkheden:
* Productprofielen maken en beheren.
* Machtigingen en functietoegang toewijzen binnen profielen.
* Voeg gebruikers toe of verwijder gebruikers binnen profielen.

  **Best voor:** de leiden van het Departement of teammanagers die kleinere groepen met gespecialiseerde behoeften controleren

  Beheerders kunnen rollen combineren voor meer flexibiliteit, afhankelijk van organisatorische vereisten.

## Admin Console instellen

Om identiteit en productvergunningen voor de toepassingen van Experience Cloud te beheren, navigeer aan [ Admin Console ](https://adminconsole.adobe.com/enterprise/).

* [ de identiteit van de opstelling en enig teken-op ](https://helpx.adobe.com/enterprise/using/set-up-identity.html) - leer hoe te opstelling uw gebruikers&#39; rekeningen met verschillende types van identiteitskaart met of zonder enige sign-on (SSO). Stel SSO in voor Adobe-software, configureer SAML-instellingen en doorloop de meest voorkomende vragen en fouten.

* [ de organisatie van de opstelling via foldervertrouwen ](https://helpx.adobe.com/enterprise/using/directory-trust.html) - het foldervertrouwen van het Gebruik om uw gebruikers tegen een domein voor authentiek te verklaren dat reeds door een andere organisatie wordt geclaimd.

  Zie [ Organisaties in Experience Cloud ](organizations.md) voor informatie over organisaties.

* [ de montages van de Authentificatie (onderneming) ](https://helpx.adobe.com/enterprise/using/authentication-settings.html) - Admin Console steunt verscheidene niveaus en beleid van de wachtwoordbescherming om veiligheid en veiligheid te verzekeren. U kunt opgeven dat een beveiligingsniveau voor wachtwoorden moet worden gebruikt voor alle gebruikers in uw organisatie. Adobe Customer Care biedt drie beveiligingsniveaus.

* [ de contacten van de Privacy en van de veiligheid ](https://helpx.adobe.com/enterprise/using/security-contacts.html) - Adobe benadrukt het beschermen van de gegevens van uw organisatie en gebruikers. In het geval van een veiligheidsincident met onze softwareoplossingen, worden de meldingen verzonden naar de aangewezen nalevingsambtenaren.

  Ondernemingen hebben hun eigen personeel dat een specifieke rol speelt op het gebied van gegevensbescherming, integriteit en andere nalevingskwesties. Daarom is contactinformatie voor dergelijk personeel van essentieel belang om te helpen snelle kennisgeving in het geval van een veiligheidsincident te verzekeren.

## Gebruikersbeheer

* [ beheer veelvoudige gebruikers ](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) BulkCSV uploadt - Leer hoe te om veelvoudige gebruikers via Csv bulkupload op Adobe Admin Console te beheren.

* [ Types van Identiteit ](https://helpx.adobe.com/enterprise/using/identity.html) - De types van Identiteit staan de organisatie verschillende niveaus van controle over de rekeningen en de gegevens van gebruikers toe. Uw keuze van het identiteitsmodel is van invloed op de manier waarop uw organisatie elementen opslaat en deelt. Terwijl Federated ID- en Enterprise ID-modellen door de organisatie worden gemaakt en beheerd, worden Adobe-id&#39;s door de persoon gemaakt en beheerd.

* [ het Hulpmiddel van de Synchronisatie van de Gebruiker van de Gebruiker 1} (MOET) - het Hulpmiddel van de Synchronisatie van de Gebruiker van Adobe is een Desktoptoepassing die wordt gebruikt om het proces te automatiseren om gebruikersgegevens tussen het systeem van het identiteitsbeheer van een organisatie (als Actieve Folder) en Adobe Adobe Admin Console te synchroniseren. ](https://helpx.adobe.com/enterprise/using/user-sync.html) Met dit hulpprogramma kunnen beheerders provisioning, updates en deactivering van gebruikers in Adobe-producten stroomlijnen.

  Met het hulpprogramma Gebruikerssynchronisatie kunnen organisaties het beheer van gebruikersaccounts en licenties vereenvoudigen door gebruikersgegevens (zoals rollen, groepen en toegangsrechten) automatisch te synchroniseren tussen hun directoryservice en Adobe-systemen. Dit instrument is met name handig voor bedrijven met grote teams. Het draagt bij tot het behoud van consistentie en veiligheid en zorgt ervoor dat gebruikers alleen toegang hebben tot de producten en diensten waarop zij recht hebben.

* [ de gebruikersdetails van de Mening (Hulpmiddel Admin) ](admin-tool-experience-cloud.md) - de Beheerders kunnen een sorteerbare en filterbare lijst van alle gebruikers en beleid van Experience Cloud met details in [!UICONTROL Admin Tool] bekijken.

## Rapporten en logboeken

* [ Logboek van de Controle ](https://helpx.adobe.com/enterprise/using/audit-logs.html) om alle veranderingen te volgen die in Admin Console worden aangebracht.

Voor hulp die niet in de voorafgaande plaatsen wordt beschreven, doorblader de [ gids van de Onderneming en van teamadmin ](https://helpx.adobe.com/nl/enterprise/admin-guide.html).

## Toepassingsspecifieke bronnen

Met deze koppelingen vindt u beheerinformatie voor specifieke Experience Cloud-toepassingen.

<!-- | Application | Link to resource|
| ------- | ------- |
|  [!DNL Analytics] <p>Customer Journey Analytics| [Analytics in the Adobe Admin Console overview](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) <p>[Administration requirements](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) |
| [!DNL Audience Manager] | [Audience Manager user migration to Admin Console](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) |
| [!DNL Campaign] v8 |  [Get started with permissions](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) |
| [!DNL Campaign Standard] to [!DNL Campaign v8] | [User access management from Campaign Standard to Campaign V8](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) |
| [!DNL Commerce] | [Configure the Commerce Admin Integration with Adobe ID](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) |
| [!DNL Dynamic Media Classic] | [Administration setup](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) |
| [!DNL Experience Manager as a Cloud Service] |  [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) |
| [!DNL Experience Platform] <p>[!DNL Data Collection] | [Access control UI overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) <p>[Permission management for data collection in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)|
| [!DNL GenStudio for Performance Marketing] | [Provision Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) |
| [!DNL Journey Optimizer] | [Manage users and roles](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) |
| [!DNL Journey Optimizer B2B Edition] | [User management](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) |
|[!DNL  Journey Orchestration] | [Access management](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) |
| [!DNL Marketo Engage] | [Understanding Marketo Subscription and User Migration to the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) |
| [!DNL Marketo Measure] | [Adobe Admin Console Setup](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) |
| [!DNL Mix Modeler] | [Access controls](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls) |
| [!DNL Pass] | [Get started with Account IQ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started) |
| [!DNL Target] | [Administrator first steps](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target) <p> [User management](https://experienceleague.adobe.com/en/docs/target/using/administer/manage-users/user-management) |
| [!DNL Workfront] | [Manage users in the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console) |

 -->

* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace)
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration)
* [Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions)
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs)
* [ Commerce ](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config)
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration)
* [ Experience Manager as a Cloud Service ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console)
* [ Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) en [ de Inzameling van Gegevens ](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [ GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning)
* [ Journey Optimizer ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [ Journey Optimizer B2B edition ](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management)
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management)
* [ Marketo Engage ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console)
* [ Marketo Measure ](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup)
* [ Mix Modeler ](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [ Adobe Pass ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started)
* [ Doel ](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [ Workfront ](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)