---
description: Leer meer over de Experience Cloud Admin Tool om een sorteerbare en filterbare lijst met alle Experience Cloud-gebruikers weer te geven.
keywords: core services
seo-description: Leer meer over de Experience Cloud Admin Tool om een sorteerbare en filterbare lijst met alle Experience Cloud-gebruikers weer te geven.
seo-title: Gebruikers van de cloud en gebruikersgegevens weergeven
solution: Experience Cloud
title: 'Gebruikers van de cloud en gebruikersgegevens weergeven '
index: true
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Gebruikers van de cloud weergeven in het beheerprogramma

Beheerders kunnen een sorteerbare en filterbare lijst weergeven met alle gebruikers van de Experience Cloud en hun gegevens in het Admin Tool. De details van de gebruiker omvatten de het producttoegang van een gebruiker, rollen, en laatste betreden informatie. (**Opmerking:** Gebruiker- en productbeheer is geconfigureerd in de [beheerconsole](admin-getting-started.md).)

1. Aanmelden bij `https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Klik in de startpagina van Experience Cloud op **[!UICONTROL Admin Tool.]**

   (U kunt _home_ ook vervangen door _admin in de URL van de homepage._)

   De pagina [!UICONTROL Gebruikers] wordt weergegeven.

## Gebruikerspagina

Deze pagina bevat een volledige lijst met gebruikers die toegang hebben tot Experience Cloud in uw organisatie. Het verstrekt informatie over oplossingsbevoegdheid en laatste login. U kunt zoeken, sorteren en filteren op aangepaste weergaven van de gebruikerslijst.

![](assets/admin-tool-users.png)

| Element | Beschrijving |
|---|---|
| [!UICONTROL Naam] | De voornaam en achternaam van de gebruiker. U kunt deze kolom sorteren van A tot Z en van Z tot A.  Klik op de naam van een gebruiker voor meer informatie over de gebruiker. |
| [!UICONTROL E-mail] | Het e-mailadres dat aan de gebruiker is gekoppeld. Kolom kan A->Z, Z->A worden gesorteerd. |
| [!UICONTROL Type id] | Het identiteitstype voor de account van de gebruiker. Filter kan worden toegepast op weergavespecifieke id-typen. Zie Identiteitstypen [](https://helpx.adobe.com/enterprise/using/identity.html) beheren voor meer informatie. |
| [!UICONTROL Oplossingen] | Overzicht van Experience Cloud-oplossingen waartoe de gebruiker toegang heeft. U kunt filters op versmalde benedenlijst van gebruikers met specifieke oplossingstoegang toepassen. |
| [!UICONTROL Laatste aanmelding] | Tijd en datum van de meest recente gebruikersaanmelding bij de Experience Cloud. Deze kolom kan worden gesorteerd op oplopende of aflopende datums. <br> **Belangrijk:** Vanaf 13 januari 2020 worden de laatste aanmeldingsgegevens van een gebruiker 365 dagen bewaard. Deze informatie is bedoeld om de huidige aanmeldingsactiviteiten in de Experience Cloud weer te geven en niet om een aanbeveling te doen om vóór 13 januari 2020 actie te ondernemen met betrekking tot inactieve accounts. |

## De weergave van de gebruikerslijst aanpassen

U kunt de kolommen doorzoeken, sorteren of filteren om de gebruikerslijst aan te passen.

* Zoeken naar gebruikers op naam of e-mail. Zoekopdrachten komen overeen met de tekenreeks die u typt.
* Sorteer de kolom door waarden op te nemen of af te nemen. Dit geldt voor de kolommen [!UICONTROL Naam,] [!UICONTROL E-mail,] [!UICONTROL Laatste aanmelding] .
* Klik op het pictogram **[!UICONTROL Filteren op]** om meerdere filters toe te passen op gebruikers met specifieke criteria. Wanneer er meerdere filtercategorieën worden toegepast, bevatten zoekopdrachten e-maildomein- `AND` id- `AND` oplossing.

| Element | Beschrijving |
|---------|----------|
| [!UICONTROL E-maildomein] , filter | Zoeken naar tekenreeksen in de kolom E-mail om de resultaten te beperken tot een of meerdere domeinen. Meerdere filters toevoegen door op Enter te drukken na elke zoekterm |
| [!UICONTROL ID-type] , filter | Maak een keuze uit beschikbare id-typen. Meerdere id-typen kunnen als filter worden gebruikt. |
| [!UICONTROL Oplossing] , filter | Kies uit beschikbare oplossingen. De veelvoudige oplossingsfilters zoeken naar resultaten die Oplossing 1 `OR` Oplossing 2 bevatten. |

## Gebruikersgegevens weergeven

Klik op de e-mail van de gebruiker op de pagina [!UICONTROL Gebruikers] om de gegevens van de gebruiker weer te geven.

![](assets/admin-tool-user-details.png)

Een gedetailleerde mening van elke gebruiker toont belangrijke details over de de oplossingstoegang van de gebruiker, admin en productrollen, en laatste betreden informatie.

## Info over Sectie

In deze sectie wordt een overzicht van de gebruikersaccount weergegeven, waaronder:

* Avatar gebruiker en de Badge van de Admin van het Systeem (indien van toepassing)
* Naam
* E-mail
* Gebruikersnaam (gebruikersnamen van een gefedereerde id-account verschillen mogelijk van die van het e-mailadres)
* [Type id](https://helpx.adobe.com/enterprise/using/identity.html)
* Land
* Laatste aanmelding

## Overzicht van oplossingen

In deze sectie wordt een overzicht weergegeven van de oplossingen van Experience Cloud waartoe de gebruiker toegang heeft. Omvat, indien van toepassing, de administratieve rol van het product

## Lijst met gedetailleerde producttoegang

In deze sectie wordt een volledige lijst weergegeven met alle productprofielen die zijn toegewezen aan de gebruiker.

| Element | Beschrijving |
|---------|----------|
| [!UICONTROL Product] | Naam van het product dat aan het productprofiel is gekoppeld. |
| [!UICONTROL Instantie] | Naam van het exemplaar (zoals login bedrijf of huurder) verbonden aan het product en productprofiel. |
| [!UICONTROL Productprofiel] | Unieke naam van het productprofiel. |
| [!UICONTROL Toegewezen door groep] | Naam van de Gebruikersgroep die de gebruiker aan een productprofiel associeert. Lege resultaten geven aan dat de gebruiker rechtstreeks en niet via een groep aan het productprofiel is toegewezen. |
| [!UICONTROL Productrollen] | Roltoewijzing van de gebruiker binnen het productprofiel. Deze informatie is momenteel alleen van toepassing op Adobe Target-productprofielen. |
