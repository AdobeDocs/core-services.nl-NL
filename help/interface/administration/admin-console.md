---
title: Licentiebeheer voor gebruikers en producten
description: Gebruikers en productlicenties beheren in Admin Console voor Experience Cloud-toepassingen.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: ce65c5292caaa4a24945e2119e78fd97a7d84109
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 5%

---

# Gebruikersbeheer en productlicenties

U kunt gebruikers en productvergunningen in Adobe [ Admin Console ](https://adminconsole.adobe.com/enterprise/) beheren. Voor algemene hulp van het identiteitsbeheer toepasselijk op alle toepassingen van Adobe, zie de [ gids van de Onderneming en van teamadmin ](https://helpx.adobe.com/nl/enterprise/admin-guide.html).

Deze pagina verstrekt informatie specifiek nuttig voor de beheerders van Experience Cloud, bepaalt rollen, en verzekert verbindingen met gemeenschappelijke gebruikers en productbeheeronderwerpen in de ondernemingsgids.

## Administratieve taken in Admin Console

De Admin Console biedt drie primaire administratieve taken, elk met specifieke niveaus van toegang en verantwoordelijkheid:

| Rol | Beschrijving |
| ------- | ------- |
| Systeembeheerder | Volledige toegang - Beheert alle aspecten van de console. <br> Belangrijkste verantwoordelijkheden: <br><ul><li>Gebruikers toevoegen, verwijderen en beheren.</li><li>Productlicenties toewijzen en intrekken.</li><li>Identiteitsinstellingen en verificatiemontages configureren</li><li>Factureringsgegevens weergeven en beheren.</li><li>Stel aanvullende beheerders en gedelegeerde rollen in.</li></ul> **Best voor:** de beheerders of het team van IT leiden die het milieu van Adobe van de volledige organisatie controleren. |
| Productbeheerder | Product-specifiek beheer - controleert toegang en toestemmingen voor specifieke producten van Adobe.<br> Zeer belangrijke verantwoordelijkheden:<ul><li>Licenties toewijzen en beheren voor een specifiek product.</li><li>Productprofielen maken en beheren.</li><li>Voeg of verwijder gebruikers binnen toegewezen producten toe.</li></ul>   **Best voor:** Teams/gebruikers die specifieke software zoals Marketo Engage of Adobe Creative Cloud beheren. |
| Beheerder van productprofiel | Korrelig rolbeheer - concentreert zich op het beheren van gebruikersgroepen en toestemmingen binnen een product.<br> Zeer belangrijke Verantwoordelijkheden:<ul><li>Productprofielen maken en beheren.</li><li>Machtigingen en functietoegang toewijzen binnen profielen.</li><li>Voeg gebruikers toe of verwijder gebruikers binnen profielen.</li></ul> **Best voor:** de leiden van het Departement of teammanagers die kleinere groepen met gespecialiseerde behoeften controleren. <br> Beheerders kunnen rollen combineren voor meer flexibiliteit, afhankelijk van organisatorische vereisten. |

## Admin Console voor Experience Cloud

Om identiteit en productvergunningen voor de toepassingen van Experience Cloud te beheren, navigeer aan [ Admin Console ](https://adminconsole.adobe.com/enterprise/).

Hier zijn middelen u zou kunnen nodig hebben wanneer het worden begonnen als beheerder in Admin Console:

### Bronnen instellen

| Help-koppeling | Beschrijving |
| ------- | ------ |
| [ de identiteit van de opstelling en enig teken-op ](https://helpx.adobe.com/enterprise/using/set-up-identity.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Settings]** <br> Leer hoe u gebruikersaccounts instelt met verschillende id-typen met of zonder SSO (Single Sign-On). Stel SSO in voor Adobe-software, configureer SAML-instellingen en doorloop de meest voorkomende vragen en fouten. |
| [ de organisatie van de opstelling via foldervertrouwen ](https://helpx.adobe.com/enterprise/using/directory-trust.html) | Verifieer uw gebruikers tegen een domein dat reeds door een andere organisatie wordt geclaimd. Voor informatie over het vinden van en het schakelen van organisaties, zie [ Organisaties in Experience Cloud ](organizations.md). |
| [ de montages van de Authentificatie (onderneming) ](https://helpx.adobe.com/enterprise/using/authentication-settings.html) | Admin Console ondersteunt verschillende wachtwoordbeveiligingsniveaus en -beleid om de veiligheid en beveiliging te waarborgen. U kunt opgeven dat een beveiligingsniveau voor wachtwoorden moet worden gebruikt voor alle gebruikers in uw organisatie. |
| [ De contacten van de Privacy en van de veiligheid ](https://helpx.adobe.com/enterprise/using/security-contacts.html) | Bescherm de gegevens van uw organisatie en gebruikers. Als zich een beveiligingsincident met onze softwareoplossingen voordoet, worden meldingen verzonden naar de juiste compatibiliteitsagenten. Ondernemingen hebben personeel dat een specifieke rol speelt op het gebied van gegevensbescherming, integriteit en andere nalevingskwesties. Daarom is contactinformatie voor dergelijk personeel van essentieel belang om te helpen snelle kennisgeving in het geval van een veiligheidsincident te verzekeren. |

### Gebruikersbeheer

| Help-koppeling | Beschrijving |
| ------- | ------- |
| [ beheer veelvoudige gebruikers ](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Users]** <br> Leer hoe u meerdere gebruikers kunt beheren via CSV-bulkupload naar de Admin Console. |
| [ Types van Identiteit ](https://helpx.adobe.com/enterprise/using/identity.html) | De types van identiteit staan de organisatie verschillende niveaus van controle over de rekeningen en de gegevens van de gebruikers toe. Uw keuze van het identiteitsmodel is van invloed op de manier waarop uw organisatie elementen opslaat en deelt. Terwijl Federated ID- en Enterprise ID-modellen door de organisatie worden gemaakt en beheerd, worden Adobe-id&#39;s door de persoon gemaakt en beheerd. |
| [ het Hulpmiddel van de Synchronisatie van de Gebruiker ](https://helpx.adobe.com/enterprise/using/user-sync.html) (MOET) | Het Adobe-hulpprogramma voor gebruikerssynchronisatie is een bureaubladtoepassing waarmee de synchronisatie van gebruikersgegevens tussen het identiteitsbeheersysteem van een organisatie (zoals Active Directory) en Adobe Admin Console wordt geautomatiseerd. Met dit hulpprogramma kunnen beheerders provisioning, updates en deactivering van gebruikers in Adobe-producten stroomlijnen. |
| [ de gebruikersdetails van de Mening (Hulpmiddel Admin) ](admin-tool-experience-cloud.md) | Bekijk een sorteerbare en filterbare lijst met alle Experience Cloud-gebruikers en -beleidsregels met informatie in de [!UICONTROL Admin Tool] . |

### Rapporten en logboeken

| Help-koppeling | Beschrijving |
| ------- |------- |
| [ Logboek van de Controle ](https://helpx.adobe.com/enterprise/using/audit-logs.html) | **[!UICONTROL Insights]** > **[!UICONTROL Logs]** > **[!UICONTROL Audit Log]** <br> Alle in de Admin Console aangebrachte wijzigingen bijhouden. |


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

Het grootste deel van Admin Consol hulp voor alle toepassingen van Adobe wordt gedocumenteerd in [ gids van de Onderneming en van teamadmin ](https://helpx.adobe.com/nl/enterprise/admin-guide.html).
