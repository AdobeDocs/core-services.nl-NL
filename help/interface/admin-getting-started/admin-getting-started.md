---
description: Leer hoe u zich aanmeldt bij de beheerconsole, gebruikersmachtigingen en productprofielen voor Experience Cloud beheert en browserondersteuning.
keywords: core services
seo-description: Leer hoe u zich aanmeldt bij de beheerconsole, gebruikersmachtigingen en productprofielen voor Experience Cloud beheert en browserondersteuning.
seo-title: Gebruikers en producten van Experience Cloud beheren
solution: Experience Cloud
title: Gebruikers en producten van Experience Cloud beheren
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: tm+mt
source-git-commit: 5e57aedb38e6914f7e99b1b26df9e4bb52b9e13d

---


# Gebruikers en producten van Experience Cloud beheren {#topic_3FCB4099640647E3B2411ADBFCE81909}

Leer hoe u zich aanmeldt bij de beheerconsole, gebruikersmachtigingen en productprofielen voor Experience Cloud beheert en browserondersteuning.

>[!IMPORTANT]
>
>Gebruikers beheren in de beheerconsole introduceert nieuwe termen, interfaces en navigatie. De volgende informatie beschrijft deze veranderingen en verzekert verbindingen aan extra hulpmiddelen. Deze Help vormt een aanvulling op de informatie in de [Enterprise Administration User Guide](https://helpx.adobe.com/enterprise/managing/user-guide.html) voor alle Adobe-cloudproducten.

## Nieuw in Experience Cloud-gebruikersbeheer {#concept_06A0A13362F644FB90F947238407637A}

Meer informatie over de nieuwste functies in Experience Cloud-gebruikersbeheer.

## Aanmelden bij de beheerconsole {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Beheerders beheren gebruikers niet meer in oplossingen. Gebruiker- en productbeheer voor Experience Cloud vindt nu plaats in de beheerconsole.

**Aanmelden bij de beheerconsole**

1. Ga naar [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Typ uw [Adobe-id of Enterprise-id](https://helpx.adobe.com/enterprise/help/identity.html) en wachtwoord.

Of klik in het menu Experience Cloud ( ![](assets/menu-icon.png)) op **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]**.

**Gerelateerde help**

[Gebruikershandleiding](https://helpx.adobe.com/enterprise/using/users.html) voor beheer voor Creative Cloud en Document Cloud. Bepaalde informatie is relevant voor het gebruikersbeheer van Experience Cloud, zoals het [beheren van identiteitstypen](https://helpx.adobe.com/enterprise/help/identity.html).

[Meld u aan en beheer uw profielinstellingen](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) om wachtwoorden, organisaties en meldingen te beheren.

## Productprofielen en -groepen {#section_AB50558124D541CF80A0D3D76D35A4BF}

De toevoeging van productprofielen markeert een verschuiving van hoe de oplossingsproducten en de diensten eerder werden beheerd (door groepen te gebruiken). In de beheerconsole zijn machtigingen gebaseerd op productprofielen. Dit zijn groepen producten en services die u aan gebruikers kunt toewijzen.

Bijvoorbeeld in Analytics, kunt u een inzameling van rapporteringshulpmiddelen, zoals de Werkruimte van de Analyse en de Bouwer van het Rapport, samen met rapportsuites, metriek, dimensies, etc. vormen. U kunt gebruikers toegang geven tot een productprofiel door ze aan het profiel toe te voegen. Zie Toegangsrechten voor Analytics [toewijzen aan een productprofiel](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Gerelateerde help**

[Beperkte beheerrechten delegeren](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analyse {#section_97DE101F92CD494AB073893680992F1A}

De gebruikers- en productmachtigingen van Analytics beheren in de beheerconsole.

[Toestemmingen van de toegang van Analytics aan een productprofiel](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)(op deze pagina) toewijzen.

**Migratie van gebruikersaccount**

Er is een hulpprogramma voor het migreren van gebruikers-id&#39;s voor Analytics-beheerders beschikbaar waarmee u gebruikersaccounts kunt migreren van Analytics User Management naar de [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

De accountmigratie wordt in fasen uitgevoerd naar klanten. Adobe brengt u op de hoogte en helpt u wanneer het uw tijd is om bestaande gebruikersaccounts te migreren van **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** naar de beheerconsole.

Na de migratie melden gebruikers zich aan met hun Adobe-id (of Enterprise-id) en verifiëren ze zich op [Experience Cloud-oplossingen en -services op ExperienceCloud.adobe.com](https://experiencecloud.adobe.com). Als gebruikers proberen zich aan te melden via oude logins ([!DNL my.omniture.com] en [!DNL sc.omniture.com]), worden ze doorgestuurd naar [!DNL experiencecloud.adobe.com].

**Gerelateerde help**

[Migratie van gebruikers-id voor analyse](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Doel - productprofielen versus werkruimten {#section_3860AF177C9E4C7E9C390D36A414F353}

In Doel is een werkruimte een productprofiel. Het laat een organisatie een specifieke reeks gebruikers aan een specifieke reeks eigenschappen toewijzen. In veel opzichten is een werkruimte vergelijkbaar met een rapportsuite in Adobe Analytics.

Zie:
* [Machtigingen voor zakelijke gebruikers](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* Video: [Hoe te om de Werkruimten van het Doel in de Console van Adobe te vormen Admin](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campagne - productprofielen, huurders en veiligheidsgroepen {#section_09CDF75366444CF5810CF321B7C712F3}

Een *huurder* in Campagne toont als *product* in de pagina van de Producten van de Console Admin.

*Beveiligingsgroep* wordt weergegeven als een productprofiel.

Zie [Groepen en gebruikers](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) beheren voor informatie over beveiligingsgroepen en gebruikers toewijzen aan beveiligingsgroepen.

## Introductie van Experience Platform {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch wordt weergegeven op de pagina Producten in de beheerconsole. U kunt andere oplossingen en de diensten in een het productprofiel van de Lancering omvatten.

Zie [Gebruikersbeheer](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) voor informatie over gebruikersmachtigingen in de beheerconsole en stel Starten-specifieke opties in, waaronder het toewijzen van rechten aan profielen.

## Dynamisch tagbeheer {#section_3A41CF2BD5994B9891537D063571D4ED}

Gebruikers uitnodigen voor dynamisch tagbeheer en gebruikersrollen toewijzen en gebruikers toevoegen aan groepen.

Zie [Gebruikers en Toestemmingen](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) voor informatie over hoe te om gebruikers aan Dynamisch Beheer van de Markering uit te nodigen en gebruikersrollen toe te wijzen en gebruikers aan groepen toe te voegen.

## Auditiebeheer {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Maak gebruikers van Audience Manager en wijs deze toe aan groepen. U kunt ook limieten (kenmerken, segmenten, doelen en AlgoModel) weergeven.

Zie [Beheer](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) in de Help van Audience Manager.

## Experience Cloud-producten beheren {#task_16335111C52D40E9BAC73D0699584DBF}

Maak een productprofiel en wijs dit toe aan een machtigingengroep.

Wanneer u een gebruiker naar een organisatie uitnodigt, kunt u de gebruiker toegang geven tot producten en productprofielen. U kunt beperkte administratieve toestemmingen aan een gebruiker ook delegeren. Op dezelfde manier kunt u gebruikersgroepen creëren, dan de groep toevoegen aan een productprofiel om toegang toe te laten.

1. Klik in de [beheerconsole](https://adminconsole.adobe.com/enterprise/)op **[!UICONTROL Products]**.
1. Klik op **[!UICONTROL New Profile]**.
1. Configureer de profieldetails en klik vervolgens op **[!UICONTROL Next]**.
1. Klik op **[!UICONTROL Done]**.

Meer hulp is beschikbaar op:

* [Producten en profielen beheren](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [De Toestemmingen](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) van de Gebruiker van de onderneming in de Hulp van het Doel voor meer informatie.
* Video: [Hoe te om de Werkruimten van het Doel in de Console van Adobe te vormen Admin](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Toestemmingen van de toegang van Analytics aan een productprofiel toewijzen {#task_040673FE3E3E429B9531FBCB8B6A4391}

Wijs Analytics de toestemmingen van de rapporttoegang (rapportreeksen, metriek, dimensies, etc.) aan een productprofiel toe.

U kunt bijvoorbeeld een productprofiel maken dat meerdere analyseprogramma&#39;s ( [!UICONTROL Analysis Workspace], [!UICONTROL Reports & Analytics]en [!UICONTROL Report Builder]) bevat, met toestemming voor specifieke metriek en dimensies (inclusief eVars) en mogelijkheden zoals het maken van segmenten of berekende metriek.

1. Meld u aan bij de [beheerconsole](https://adminconsole.adobe.com/enterprise)en klik op **[!UICONTROL Products]** (of klik op de naam van het product).
1. Klik in het productprofiel op **[!UICONTROL Permissions]** (alleen beschikbaar voor beheerders).
1. De profielmachtigingen configureren:

| Element | Beschrijving |
|--- |--- |
| Rapportageopties | Schakel machtigingen in voor specifieke rapportsuites. |
| Metrisch | Laat toestemmingen voor verkeer, omzetting, douanegebeurtenissen, oplossingsgebeurtenissen, bewuste inhoud toe, etc. |
| Afmetingen | Pas gebruikerstoegang op een korrelig niveau, met inbegrip van eVars, verkeersrapporten, oplossingsrapporten, en het kleven rapporten aan. |
| Rapportsuite-gereedschappen | Schakel gebruikersmachtigingen in voor webservices, rapportbeheer, tools en rapporten en dashboarditems. |
| Analysegereedschappen | Laat gebruikerstoestemmingen voor Algemene punten (het factureren, logboeken, enz.), het Beheer van het Bedrijf, Hulpmiddelen, de Toegang van de Dienst van het Web, de Bouwer van het Rapport, en de integratie van de Verbindingen van Gegevens toe. De bedrijfsinstellingen van de categorie Admin Console aanpassen zijn verplaatst naar Analytics Tools. |

## Beheerdersrollen delegeren aan gebruikers {#task_3A072C4AA9734BC59FFA7E015271BC7E}

In de beheerconsole kunt u beperkte beheerrechten delegeren aan anderen in uw organisatie. Met gedelegeerde rollen kunnen gebruikers softwaretoegang voor eindgebruikers beheren, toegangsimplementatiemogelijkheden bieden en als ondersteuningsafgevaardigden functioneren.

U kunt bijvoorbeeld:

* Creative Cloud toegankelijk maken voor Creative Cloud.
* Laat uw marketingdirecteur toegang verlenen tot de Experience Cloud.
* Houd deze twee rollen afzonderlijk zodat kunnen zij elkaars rollen niet overstappen.

Door deze rollen te gebruiken, kunt u beheer aan anderen gelijktijdig delegeren zonder meer vermogen te verstrekken dan zij nodig hebben.

1. Klik in de beheerconsole op **[!UICONTROL Users]** de naam van de gebruiker.
1. Klik op **[!UICONTROL Edit admin rights]**.
1. Configureer de beheerdersrechten van de gebruiker.
1. Klik **[!UICONTROL Next]** om de instellingen te bekijken en klik vervolgens op **[!UICONTROL Save]**.

## Ondersteunde browsers en systeemvereisten {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Ondersteunde browsers in de Experience Cloud.

Tot de volgende browsers behoren browsers die via Experience Cloud worden ondersteund:

* [!DNL Microsoft Edge] (Microsoft heeft de ondersteuning [voor Internet Explorer 8, 9 en 10](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) beëindigd. Adobe lost de problemen die zijn gemeld voor deze specifieke versies van Internet Explorer dan ook niet op.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Opmerking:** Hoewel de interface Experience Cloud deze browsers ondersteunt, wordt mogelijk niet elke browser ondersteund door afzonderlijke oplossingen. ( [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html) biedt bijvoorbeeld geen ondersteuning [!DNL Opera]en [Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html) biedt geen ondersteuning voor [!DNL Safari].)

**Oplossing en productvereisten**

* [Analyse](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe-doel](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
