---
description: Leer hoe u zich aanmeldt bij de Adobe Admin Console, gebruikersmachtigingen en productprofielen voor Experience Cloud beheert en browserondersteuning.
keywords: Experience Cloud services
solution: Experience Cloud
title: 'Leer hoe u gebruikers en producten beheert '
index: true
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 5%

---


# Gebruikers en producten van Experience Cloud beheren {#topic_3FCB4099640647E3B2411ADBFCE81909}

Leer hoe u zich aanmeldt bij de Admin Console, gebruikersmachtigingen en productprofielen voor Experience Cloud beheert en browserondersteuning.

>[!IMPORTANT]
>
>Het leiden van gebruikers in de Admin Console introduceert nieuwe termijnen, interfaces, en navigatie. De volgende informatie beschrijft deze veranderingen en verzekert verbindingen aan extra hulpmiddelen. Deze Help vormt een aanvulling op de informatie in de gebruikershandleiding [voor](https://helpx.adobe.com/nl/enterprise/managing/user-guide.html) bedrijfsbeheer voor alle Adobe-cloudproducten.

## Nieuw in Experience Cloud-gebruikersbeheer {#concept_06A0A13362F644FB90F947238407637A}

Meer informatie over de nieuwste functies in het gebruikersbeheer van Experience Cloud.

<!-- ### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

### Beheer

Beheerders kunnen een sorteerbare en filterbare lijst met alle Experience Cloud-gebruikers en hun gegevens weergeven in het Admin Tool. Zie Experience Cloud-gebruikers [weergeven in het gereedschap](admin-tool-experience-cloud.md)Beheer.

## Aanmelden bij de Admin Console {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Beheerders beheren gebruikers niet meer in oplossingen. Gebruiker- en productbeheer voor Experience Cloud vindt nu plaats in de Admin Console.

Aanmelden bij de Admin Console:

1. Ga naar [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Typ uw [Adobe ID of Enterprise ID](https://helpx.adobe.com/enterprise/help/identity.html) en wachtwoord.

U kunt ook in het menu Experience Cloud ( ![](assets/menu-icon.png)) op **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]** klikken.

**Gerelateerde help**

[Gebruikershandleiding](https://helpx.adobe.com/nl/enterprise/using/users.html) voor het beheer van de Creative Cloud en het Document Cloud. Sommige informatie is relevant voor het beheer van Experience Cloud-gebruikers, zoals het [beheren van identiteitstypen](https://helpx.adobe.com/enterprise/help/identity.html).

[Meld u aan en beheer uw profielinstellingen](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) om wachtwoorden, organisaties en meldingen te beheren.

## Productprofielen en -groepen {#section_AB50558124D541CF80A0D3D76D35A4BF}

De toevoeging van productprofielen markeert een verschuiving van hoe de oplossingsproducten en de diensten eerder werden beheerd (door groepen te gebruiken). In de Admin Console, zijn de toestemmingen gebaseerd op productprofielen, die groepen producten en de diensten zijn die u aan gebruikers kunt toewijzen.

Bijvoorbeeld in Analytics, kunt u een inzameling van rapporteringshulpmiddelen, zoals Analysis Workspace en Report Builder, samen met rapportsuites, metriek, afmetingen, etc. vormen. U kunt gebruikers toegang geven tot een productprofiel door ze aan het profiel toe te voegen. Zie Toegangsrechten voor Analytics [toewijzen aan een productprofiel](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Gerelateerde help**

[Beperkte beheerrechten delegeren](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

De gebruikers- en productmachtigingen voor Analytics beheren in de Admin Console.

[Toestemmingen van de toegang van Analytics aan een productprofiel](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)(op deze pagina) toewijzen.

**Migratie van gebruikersaccount**

Er is een hulpprogramma voor het migreren van gebruikers-id&#39;s voor Analytics-beheerders beschikbaar waarmee u gebruikersaccounts kunt migreren van Analytics User Management naar [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

De accountmigratie wordt in fasen uitgevoerd aan klanten. Adobe geeft een melding en helpt u wanneer het uw tijd is om bestaande gebruikersaccounts van **[!UICONTROL Admin Tools]** > naar de Admin Console te migreren. U kunt dan ook **[!UICONTROL User Management]** het volgende doen.

Na de migratie melden gebruikers zich aan met hun Adobe ID (of Enterprise ID) en verifiëren ze hun Experience Cloud-oplossingen en -services op [ExperienceCloud.adobe.com](https://experiencecloud.adobe.com). Als gebruikers proberen zich aan te melden via oude logins ([!DNL my.omniture.com] en [!DNL sc.omniture.com]), worden ze doorgestuurd naar [!DNL experiencecloud.adobe.com].

**Gerelateerde help**

[Migratie van gebruikers-id voor analyse](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Adobe Target - productprofielen versus werkruimten {#section_3860AF177C9E4C7E9C390D36A414F353}

In Adobe Target is een werkruimte een productprofiel. Het laat een organisatie een specifieke reeks gebruikers aan een specifieke reeks eigenschappen toewijzen. In veel opzichten is een werkruimte vergelijkbaar met een rapportsuite in Adobe Analytics.

Zie:

* [Machtigingen voor zakelijke gebruikers](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* Video: [Adobe Target-werkruimten configureren in Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campagne - productprofielen, huurders en veiligheidsgroepen {#section_09CDF75366444CF5810CF321B7C712F3}

Een *huurder* in Campagne toont als *product* in de pagina van de Producten van de Admin Console.

*Beveiligingsgroep* wordt weergegeven als een productprofiel.

Zie [Groepen en gebruikers](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) beheren voor informatie over beveiligingsgroepen en gebruikers toewijzen aan beveiligingsgroepen.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch wordt weergegeven op de pagina Producten in de Admin Console. U kunt andere oplossingen en de diensten in een het productprofiel van de Lancering omvatten.

Zie [Gebruikersbeheer](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) voor meer informatie over gebruikersmachtigingen in de Admin Console en stel Starten-specifieke opties in, waaronder het toewijzen van rechten aan profielen.

## Experience Manager as a Cloud Service

Adobe Enterprise-klanten worden vertegenwoordigd als IMS-organisaties in de Adobe Admin Console. Dit is het portaal dat door klanten van de Adobe wordt gebruikt om hun productrechten voor hun gebruikers en groepen te beheren. AEM klanten kunnen de Adobe Admin Console gebruiken om hun productrechten te beheren en IMS-verificatie om als Cloud Service te AEM.

See [IMS Support for AEM as a Cloud Service](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/security/ims-support.html#managing-products-and-user-access-in-admin-console).

## Dynamisch tagbeheer {#section_3A41CF2BD5994B9891537D063571D4ED}

Gebruikers uitnodigen voor dynamisch tagbeheer en gebruikersrollen toewijzen en gebruikers toevoegen aan groepen.

Zie [Gebruikers en Toestemmingen](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) voor informatie over hoe te om gebruikers aan Dynamisch Beheer van de Markering uit te nodigen en gebruikersrollen toe te wijzen en gebruikers aan groepen toe te voegen.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Maak gebruikers van Audience Managers en wijs deze toe aan groepen. U kunt ook limieten (kenmerken, segmenten, doelen en [!DNL AlgoModel]) weergeven.

Zie [Beheer](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) in de Help van de Audience Manager.

## Experience Cloud-producten beheren {#task_16335111C52D40E9BAC73D0699584DBF}

Maak een productprofiel en wijs dit toe aan een machtigingengroep.

Wanneer u een gebruiker naar een organisatie uitnodigt, kunt u de gebruiker toegang geven tot producten en productprofielen. U kunt beperkte administratieve toestemmingen aan een gebruiker ook delegeren. Op dezelfde manier kunt u gebruikersgroepen creëren, dan de groep toevoegen aan een productprofiel om toegang toe te laten.

1. Klik in de [Admin Console](https://adminconsole.adobe.com/enterprise/)op **[!UICONTROL Products]**.
1. Klik op **[!UICONTROL New Profile]**.
1. Configureer de profieldetails en klik vervolgens op **[!UICONTROL Next]**.
1. Klik op **[!UICONTROL Done]**.

Meer hulp is beschikbaar op:

* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [De Toestemmingen](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) van de Gebruiker van de onderneming in Adobe Target helpen voor meer informatie.
* Video: [Adobe Target-werkruimten configureren in Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Toestemmingen van de toegang van Analytics aan een productprofiel toewijzen {#task_040673FE3E3E429B9531FBCB8B6A4391}

Wijs Analytics de toestemmingen van de rapporttoegang (rapportreeksen, metriek, dimensies, etc.) aan een productprofiel toe.

U kunt bijvoorbeeld een productprofiel maken dat meerdere analyseprogramma&#39;s ( [!UICONTROL Analysis Workspace], [!UICONTROL Reports & Analytics]en [!UICONTROL Report Builder]) bevat, met toestemming voor specifieke metriek en dimensies (inclusief eVars) en mogelijkheden zoals het maken van segmenten of berekende metriek.

1. Meld u aan bij de [Admin Console](https://adminconsole.adobe.com/enterprise)en klik op **[!UICONTROL Products]** (of klik op de naam van het product).
1. Klik in het productprofiel op **[!UICONTROL Permissions]** (alleen beschikbaar voor beheerders).
1. De profielmachtigingen configureren:

| Element | Beschrijving |
|--- |--- |
| Rapportsuites | Schakel machtigingen in voor specifieke rapportsuites. |
| Metrics | Laat toestemmingen voor verkeer, omzetting, douanegebeurtenissen, oplossingsgebeurtenissen, bewuste inhoud toe, etc. |
| Dimensies | Pas gebruikerstoegang op een korrelig niveau, met inbegrip van eVars, verkeersrapporten, oplossingsrapporten, en wegrapporten aan. |
| Rapportsuite-gereedschappen | Schakel gebruikersmachtigingen in voor webservices, rapportbeheer, tools en rapporten en dashboarditems. |
| Analysegereedschappen | Schakel gebruikersmachtigingen in voor algemene items (facturering, logbestanden, enz.), bedrijfsbeheer, tools, webservicetoegang, Report Builder en integratie van gegevensconnectors. De montages van het bedrijf van de Customize categorie van de Admin Console zijn verplaatst naar de Hulpmiddelen van Analytics. |

## Beheerdersrollen delegeren aan gebruikers {#task_3A072C4AA9734BC59FFA7E015271BC7E}

In de Admin Console, kunt u beperkte administratieve rechten aan anderen in uw organisatie delegeren. Met gedelegeerde rollen kunnen gebruikers softwaretoegang voor eindgebruikers beheren, toegangsimplementatiemogelijkheden bieden en als ondersteuningsafgevaardigden functioneren.

U kunt bijvoorbeeld:

* Laat uw creatieve regisseur toegang tot Creative Cloud verlenen.
* Laat uw marketingdirecteur toegang verlenen tot de Experience Cloud.
* Houd deze twee rollen afzonderlijk zodat kunnen zij elkaars rollen niet overstappen.

Door deze rollen te gebruiken, kunt u beheer aan anderen gelijktijdig delegeren zonder meer vermogen te verstrekken dan zij nodig hebben.

1. Klik in de Admin Console **[!UICONTROL Users]** en klik vervolgens op de naam van de gebruiker.
1. Klik op **[!UICONTROL Edit admin rights]**.
1. Configureer de beheerdersrechten van de gebruiker.
1. Klik **[!UICONTROL Next]** om de instellingen te bekijken en klik vervolgens op **[!UICONTROL Save]**.

## Ondersteunde browsers en systeemvereisten {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Ondersteunde browsers in de Experience Cloud.

* [!DNL Microsoft Edge] (Microsoft heeft de ondersteuning [voor Internet Explorer 8, 9 en 10](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) beëindigd. Als dusdanig, zal Adobe kwesties niet bevestigen die tegen deze specifieke versies van Internet Explorer worden gemeld.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Opmerking:** Hoewel de interface van Experience Cloud deze browsers steunt, zouden de individuele oplossingen niet elke browser kunnen steunen. (For example, [Analytics](https://docs.adobe.com/content/help/nl-NL/analytics/admin/sys-reqs.html) does not support [!DNL Opera], and [Adobe Target](https://docs.adobe.com/help/nl-NL/target/using/implement-target/before-implement/supported-browsers.html) does not support [!DNL Safari].)

### Oplossing en productvereisten

* [Analytics](https://docs.adobe.com/content/help/nl-NL/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/nl-NL/target/using/implement-target/before-implement/supported-browsers.html)
