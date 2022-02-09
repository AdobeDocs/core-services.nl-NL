---
title: Gebruikers en producten beheren
description: Ontdek hoe u zich aanmeldt bij de Admin Console en gebruikersmachtigingen en productprofielen voor Experience Cloud beheert. Leer over het delegeren van administratieve rechten aan Experience Cloud gebruikers, en over browser steun voor Experience Cloud.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: 3cf359c54467b4f913f20060e9d7f9577691b90c
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 2%

---

# Gebruikers en producten van Experience Cloud beheren

Leer hoe u zich aanmeldt bij de Admin Console, gebruikersmachtigingen voor Experience Cloud-gebruikers, productprofielen en browserondersteuning beheert.

>[!IMPORTANT]
>
>De volgende informatie is specifiek voor Experience Cloud toepassingen. Deze informatie vormt een aanvulling op de bredere administratieve informatie in de [Handboek voor Enterprise Administration](https://helpx.adobe.com/enterprise/admin-guide.html) voor alle Adobe cloud-producten.

U kunt een sorteerbare en filterbare lijst van alle gebruikers van de Experience Cloud en hun details in het Hulpmiddel Admin bekijken. Zie [Experience Cloud-gebruikers weergeven in het Admin-gereedschap](admin-tool-experience-cloud.md).

## Experience Cloud-gebruikersverificatie (geplande migratie){#migration}

Vanaf februari 2022 werkt Adobe zijn profielbeheersysteem bij om organisaties in staat te stellen bedrijfsrechten op individuele profielen beter te beheren. Als zodanig worden alle gebruikers met een persoonlijk profiel dat overeenkomt met een individuele Adobe ID (Type1), gemigreerd naar een nieuw bedrijfsprofiel. Dit profiel komt overeen met een _Zakelijke id_ (Type2e).

Zie [Identiteitstypen in Adobe Admin Console](https://helpx.adobe.com/enterprise/using/identity.html) voor informatie over identiteitstypen.

### Migratieproces

Wanneer het tijd is voor uw migratie, ontvangen organisatiebeheerders 30 dagen vóór de migratie een e-mail met een melding.

* De migratie zal tussen 10.00 uur worden gepland. - 6.00 uur, gebaseerd op de primaire tijdzone van de organisatie of op het weekend.
* Tijdens de migratie kan de Experience Cloud-toepassing ongeveer 15 minuten ontoegankelijk zijn en kan de Admin Console tot 30 minuten ontoegankelijk zijn. Anders verloopt deze migratie naadloos.

### Wijzigingen na de migratie

Admin Console

* Beheerders met meerdere accounts kunnen een profielkiezer zien wanneer ze zich aanmelden [!UICONTROL Admin Console].
* Individuele Adobe ID-gebruikers worden bijgewerkt naar de bedrijfs-id.
* De directory met bedrijfs-id wordt toegevoegd aan **[!UICONTROL Settings]** > **[!UICONTROL Identity]** > **[!UICONTROL Directories]**.

   ![Identiteit Admin Console - Zakelijke id](assets/identity-home.png)

### Aanmelden na migratie

Uw aanmeldingservaring verandert niet met deze update:

1. Aanmelden bij `experience.adobe.com` dezelfde referenties gebruiken.

1. Er wordt een nieuw profiel gemaakt dat is gekoppeld aan de bedrijfs-id. U wordt gevraagd **[!UICONTROL Join now]** of **[!UICONTROL Skip]**.

1. Als u een van de opties gebruikt, wordt een bestaande landingspagina weergegeven.

1. Een Adobe-profiel is gekoppeld aan elk businessplan en biedt de mogelijkheid om elementen te organiseren die zijn gemaakt op basis van extra Adobe Cloud-aanbiedingen (Creative Cloud en Document Cloud).

Zie voor meer informatie [Introductie van Adobe-profielen](https://helpx.adobe.com/enterprise/kb/introducing-adobe-profiles.html).

## Wat is een productprofiel? {#section_AB50558124D541CF80A0D3D76D35A4BF}

_[!UICONTROL Product Profiles]_Dit zijn groepen producten en services die u aan gebruikers kunt toewijzen. In Experience Cloud zijn machtigingen gebaseerd op het profiel van een product, niet op de gebruiker. (U kunt beheerrechten echter delegeren aan specifieke gebruikers.)

Bijvoorbeeld, in Analytics kunt u een inzameling van rapporteringshulpmiddelen, zoals Analysis Workspace en Report Builder, samen met rapportsuites, metriek, en dimensies vormen. U kunt toestemming verlenen aan een Profiel van het Product door gebruikers aan het profiel toe te voegen.

* See [Assign Analytics access permissions to a Product Profile](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) on this page.
* Zie [Beheerdersrollen delegeren aan gebruikers](#delegate-rights) op deze pagina

## Experience Cloud-productprofielen beheren {#task_16335111C52D40E9BAC73D0699584DBF}

U kunt een productprofiel maken en dit aan een machtigingengroep toewijzen.

Wanneer u een gebruiker naar een organisatie uitnodigt, kunt u de gebruiker toegang geven tot producten en productprofielen. U kunt beperkte administratieve toestemmingen aan een gebruiker ook delegeren. Op dezelfde manier kunt u gebruikersgroepen creëren, dan de groep toevoegen aan een Profiel van het Product om toegang toe te laten.

1. In de [Admin Console](https://adminconsole.adobe.com/enterprise/), selecteert u **[!UICONTROL Products]**.
1. Selecteer de naam van uw organisatie.
1. Selecteer **[!UICONTROL New Profile]**.
1. Configureer de profieldetails en selecteer vervolgens **[!UICONTROL Save]**.

For more information (and for help on Creative Cloud and Document Cloud product management), see [Identity](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/identity.ug.html) in the [Administration User Guide](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/users.ug.html).

**Gerelateerde help**

* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/manage-products.ug.html) in de Gebruikershandleiding voor Beheer.
* [Enterprise User Permissions](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=en) in Adobe Target help for more information.
* Video: [Adobe Target-werkruimten configureren in Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Beheerdersrollen delegeren aan gebruikers {#delegate-rights}

In the Admin Console, you can delegate limited administrative rights to others in your organization. Met gedelegeerde rollen kunnen gebruikers softwaretoegang voor eindgebruikers beheren, toegangsimplementatiemogelijkheden bieden en als ondersteuningsafgevaardigden functioneren.

U kunt bijvoorbeeld:

* Allow your creative director to grant access to Creative Cloud.
* Allow your marketing director to grant access to the Experience Cloud.
* Houd deze twee rollen afzonderlijk zodat kunnen zij elkaars rollen niet overstappen.

Door deze rollen te gebruiken, kunt u beheer aan anderen gelijktijdig delegeren zonder meer vermogen te verstrekken dan zij nodig hebben.

1. Selecteer in de Admin Console de optie **[!UICONTROL Users]** en selecteert u vervolgens de naam van de gebruiker.

   ![Administratieve rechten in Admin Console](assets/edit-admin-rights.png)

1. Selecteer **[!UICONTROL Edit admin rights]**.

   ![Bewerk de beheerrechten in Admin Console](assets/edit-admin-rights-page.png)

1. Geef de beheerdersrechten van de gebruiker op.
1. Selecteer **[!UICONTROL Save]**.

## Gebruikers en producten van Analytics beheren {#section_97DE101F92CD494AB073893680992F1A}

U kunt de toestemmingen van de het rapporttoegang van de Analyse (rapportreeksen, metriek, afmetingen, etc.) aan een Profiel van het Product toewijzen.

U kunt bijvoorbeeld een productprofiel maken dat meerdere analyseprogramma&#39;s bevat ([!UICONTROL Analysis Workspace], [!UICONTROL Reports & Analytics], en [!UICONTROL Report Builder]). Deze profielen bevatten machtigingen voor specifieke metriek en dimensies (inclusief eVars) en mogelijkheden zoals segmenten of het maken van berekende metriek.

1. Aanmelden bij de [Admin Console](https://adminconsole.adobe.com/enterprise)selecteert u vervolgens **[!UICONTROL Products]**.
1. Op de [!UICONTROL Products] pagina, selecteert u uw product en selecteert u vervolgens **[!UICONTROL Permissions]** (alleen beschikbaar voor beheerders).
1. De profielmachtigingen configureren:

| Element | Beschrijving |
|--- |--- |
| Rapportsuites | Schakel machtigingen in voor specifieke rapportsuites. |
| Metrics | Machtigingen inschakelen voor verkeer, conversie, aangepaste gebeurtenissen, toepassingsgebeurtenissen, inhoud behouden enzovoort. |
| Dimensies | Pas gebruikerstoegang op korrelig niveau, met inbegrip van eVars, verkeersrapporten, toepassingsrapporten, en wegrapporten aan. |
| Rapportsuite-gereedschappen | Schakel gebruikersmachtigingen in voor webservices, rapportbeheer, tools en rapporten en dashboarditems. |
| Analysegereedschappen | Laat gebruikerstoestemmingen voor Algemene punten (het factureren, logboeken, etc.), het Beheer van het Bedrijf, Hulpmiddelen, de Toegang van de Dienst van het Web, Report Builder, en de integratie van de Verbindingen van Gegevens toe. De montages van het bedrijf van de Customize categorie van de Admin Console zijn verplaatst naar de Hulpmiddelen van Analytics. |

**Migratie van gebruikersaccount**

Er is een hulpprogramma voor de migratie van gebruikers-id&#39;s van Analytics beschikbaar om beheerders te helpen gebruikersaccounts te migreren van Analytics User Management naar de [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

De accountmigratie wordt in fasen uitgevoerd naar klanten. Adobe brengt u op de hoogte en helpt u wanneer het uw tijd is om bestaande gebruikersaccounts te migreren van **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** aan de Admin Console.

Na de migratie melden gebruikers zich aan met hun Adobe ID (of Enterprise ID) en verifiëren ze zich bij hun Experience Cloud-toepassingen en -services op [experience.adobe.com](https://experience.adobe.com). Als gebruikers proberen zich aan te melden via oude logins ([!DNL my.omniture.com], [!DNL sc.omniture.com] en [!DNL experiencecloud.adobe.com]) worden doorgestuurd naar [!DNL experience.adobe.com].

**Gerelateerde help**

Zie voor meer informatie [Migratie van gebruikers-id voor analyse](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/migrate-users/c-migration-tool.html?lang=en)

## Adobe Target beheren - Productprofielen versus werkruimten {#section_3860AF177C9E4C7E9C390D36A414F353}

In Adobe Target is een werkruimte een productprofiel. Het laat een organisatie een specifieke reeks gebruikers aan een specifieke reeks eigenschappen toewijzen. In veel opzichten is een werkruimte vergelijkbaar met een rapportsuite in Adobe Analytics.

Zie:

* [Machtigingen voor zakelijke gebruikers](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=en)
* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/manage-products.ug.html)
* Video: [How to Configure Adobe Target Workspaces in Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campagneproductprofielen, huurders en beveiligingsgroepen beheren {#section_09CDF75366444CF5810CF321B7C712F3}

A *huurder* in Campagne wordt weergegeven als een *product* in de pagina van de Producten van de Admin Console.

*Beveiligingsgroep* wordt weergegeven als een productprofiel.

Zie [Groepen en gebruikers beheren](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=en) voor informatie over veiligheidsgroepen en het toewijzen van gebruikers aan veiligheidsgroepen.

## Gegevensverzameling van Experience Platforms beheren (starten) {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform [!UICONTROL Data Collection] ([!UICONTROL Launch]) weergegeven op de [!UICONTROL Products] pagina in de [!UICONTROL Admin Console]. U kunt andere toepassingen en services opnemen in een productprofiel starten.

Gebruikers uitnodigen om [!UICONTROL Platform Launch] en wijs gebruikersrollen en rechten toe.

Zie [Gebruikersmachtigingen](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html?lang=en) voor meer informatie over gebruikersmachtigingen in de Admin Console en over het instellen van opstartopties, waaronder het toewijzen van rechten aan profielen.

## Experience Manager as a Cloud Service

Adobe Enterprise-klanten worden vertegenwoordigd als organisaties in de Adobe [!UICONTROL Admin Console]. Experience Manager customers can use the Adobe [!UICONTROL Admin Console] to manage product entitlements and IMS authentication to Experience Manager as a [!UICONTROL Cloud Service].

Zie [IMS-ondersteuning voor as a Cloud Service Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/security/ims-support.html?lang=en).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Create Audience Manager users and assign them to groups. You can also view limits (traits, segments, destinations, and [!DNL AlgoModel]).

See [Administration](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=en) in Audience Manager help.

## Ondersteunde browsers in de Experience Cloud

* [!DNL Microsoft® Edge] (Microsoft® heeft [beëindigde ondersteuning](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) voor Internet Explorer 8, 9 en 10. Als dusdanig, lost Adobe geen kwesties op die tegen deze specifieke versies van Internet Explorer worden gemeld.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Note:** Although the Experience Cloud interface supports these browsers, individual applications do not support every browser. (Bijvoorbeeld: [Analyse](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=en) ondersteunt niet [!DNL Opera], en [Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=en) ondersteunt niet [!DNL Safari].)

### Oplossing en productvereisten

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=en)
* [Report Builder](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=en)
* [Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=en)
