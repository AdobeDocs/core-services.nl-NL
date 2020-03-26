---
description: Overwegingen en aanbevolen procedures voor het uploaden en gebruiken van persoonlijk identificeerbare informatie (PII) in de Adobe Experience Cloud.
keywords: customer attributes;core services
seo-description: Overwegingen en aanbevolen procedures voor het uploaden en gebruiken van persoonlijk identificeerbare informatie (PII) in de Adobe Experience Cloud.
seo-title: Privacyoverwegingen - klantkenmerken
solution: Experience Cloud
title: Privacyoverwegingen - klantkenmerken
uuid: 5666dc4e-55fa-4196-9985-cf530cfb9247
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Privacyoverwegingen - klantkenmerken

Overwegingen en aanbevolen procedures voor het uploaden en gebruiken van persoonlijk identificeerbare informatie (PII) in de Adobe Experience Cloud.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* Voornaam en achternaam
* Thuis of ander fysiek adres
* E-mailadres
* Telefoonnummer
* Sociale verzekeringsnummer
* Andere identificatiecode die fysieke of online contact met een persoon mogelijk maakt. (Varieert op plaats. Verifieer en volg de lokale wetten en regels met betrekking tot privacy en PII voor alle plaatsen waar u zaken doet.)


Adobe biedt tools waarmee adverteerders gedragsinformatie kunnen verzamelen over consumenten die hun sites bezoeken of hun toepassingen gebruiken. Adobe biedt ook tools waarmee adverteerders deze informatie kunnen verbeteren met offline of externe klantgegevens die de adverteerder in andere informatiemanagementsystemen kan hebben.

Een van de redenen waarom adverteerders dit doen, is het verbeteren van de informatie die beschikbaar is wanneer zij op de consument gerichte marketing- en reclamebeslissingen nemen. Met Adobe Analytics en Target kunnen adverteerders alleen persoonlijke identificeerbare gegevens (PII&#39;s), zoals e-mailadressen, uploaden nadat deze zijn gehasht om het contact met de persoon onmogelijk te maken. Onderbroken informatie kan nog steeds worden gebruikt voor analyse en marketing. Ter herinnering, Adobe verbiedt adverteerders gevoelige persoonlijke gegevens naar Adobe te verzenden, zoals medische gegevens, informatie over financiële rekeningen en informatie over minderjarigen.

Adobe beseft dat dit soort marketing- en reclamebesluiten gevolgen kan hebben voor de privacy van de consument. Daarom heeft Adobe privacycontroles ontwikkeld om adverteerders te helpen aan de verwachtingen van hun klanten te voldoen. Adobe raadt zijn adverteerders aan zorgvuldig na te denken welke informatie geschikt is voor marketingdoeleinden en onder welke omstandigheden de adverteerder toestemming heeft om dergelijke informatie te gebruiken.

**Aanbevolen procedures**

Wanneer u PII uploadt naar Adobe Analytics of Adobe Target, raadt Adobe de klant aan om PII te hashen voordat deze naar Adobe wordt geüpload. Onderbroken informatie kan nog steeds worden gebruikt voor analyse en marketing. Ter herinnering, Adobe verbiedt adverteerders gevoelige persoonlijke gegevens naar Adobe Analytics en Adobe Target te verzenden, zoals medische gegevens, informatie over financiële accounts en informatie over minderjarigen.

Adobe raadt zijn adverteerders aan zorgvuldig na te denken welke informatie geschikt is voor marketingdoeleinden en onder welke omstandigheden de adverteerder toestemming heeft om dergelijke informatie te gebruiken.

Aangezien de privacywetgeving van de consument nog steeds van kracht is, raadt Adobe aan dat adverteerders drie algemene beginselen in acht nemen:

1. Doe wat u zegt (in uw privacybeleid).
1. Zeg wat u (in uw privacybeleid) doet.
1. Verwar je consumenten niet.

Met het oog op deze verwachtingen raadt Adobe aan dat wanneer een adverteerder activiteiten aan PII koppelt, de adverteerder berichten of personalisatie verstrekt die erop wijzen dat de consument voor authentiek wordt verklaard. Een voorbeeld hiervan is het plaatsen van een begroeting in de koptekst van de website. Adobe raadt adverteerders ook aan in hun privacybeleid te beschrijven welk type bladerinformatie ze aan PII koppelen en onder welke omstandigheden ze informatie over bladeren aan PII koppelen. Tot slot raadt Adobe adverteerders ten zeerste aan de keuzemogelijkheden te bekijken die hun consumenten bieden om te begrijpen of en hoe ze de optie voor het posten van niet-geverifieerde profielgegevens kunnen gebruiken.

<!-- <p> <b>Vinay Geol</b> should help craft privacy regarding how all MAC uses privacy/cookies. Privacy implications around each part of the workflow. Moving from CRM to MAC. Can it include PII? What is PII? What isn't PII? </p> 
<p>CRM data is Known Data or Info. Going to combine with activity that occurs when visitor was not authenticated. PII wiki: </p> 
<p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> 
<p>Refactoring of implementation docs as it relates to privacy and cookies. </p> 
<p>Add content to t-publish-audience-segment, as follows: </p> 
<p> Audiences are not filtered based on the authentication state of a visitor. If a visitor can browse your site in un-authenticated and authenticated states, actions that occur when a visitor is un-authenticated can still cause a visitor to be included in an audience. Please review <link> to understand the full privacy implications of audience sharing. </p> 
<p>That "link" goes to a topic dedicated to PII, with this text: </p> 
<p> - Adobe Analytics allows its advertisers to upload personally identifiable information (PII) such as email addresses. When uploading PII to Adobe Analytics, Adobe recommends that the customer should hash PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics, such as medical records, financial account information, and information about minors. </p> 
<p> - Adobe recommends its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. </p> 
<p> - As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 1) Do what you say (in your privacy policy); 2) Say what you do (in your privacy policy); and 3) Don't surprise your consumers. </p> 
<p> - With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provide notices/personalization indicating that the consumer is authenticated. An example of this is including a 'Hello, Jane' greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt out. </p> 
<p>Possibly revamp the cookies to include privacy, with best practices: https://docs.adobe.com/content/help/en/core-services/interface/ec-cookies/cookies-privacy.html </p> -->
