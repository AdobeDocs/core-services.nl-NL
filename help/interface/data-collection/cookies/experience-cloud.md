---
description: Leer hoe de id-service wordt opgeslagen en gebruikt in Experience Cloud-toepassingen.
solution: Experience Cloud,Analytics,Target
title: Experience Cloud Cookies
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
source-git-commit: 2073400a04933226bd036c1fcd729df70f101df3
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 1%

---

# Experience Cloud cookies

Adobe Experience Cloud gebruikt cookies om een bezoeker-id op te slaan die in Experience Cloud-toepassingen wordt gebruikt. Deze koekjes zijn specifiek op de toegang tot van Adobe Experience Cloud toepassingen op [ experience.adobe.com ](https://experience.adobe.com) van toepassing.

**Naam van het Koekje: s_ecid**

<table id="table_FF4C70D3D4CC425BA65162D5A9504F7D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Kenmerk </p> </th> 
   <th colname="col2" class="entry"> <p>Beschrijving </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p> Bevat een kopie van de Experience Cloud-id (ECID) of MID. MID wordt opgeslagen in een sleutelwaardepaar dat deze syntaxis volgt, s_ecid=MCMID|&lt;ECID&gt; </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Verlopen </p> </td> 
   <td colname="col2"> <p>2 jaar, hoewel de meeste moderne browsers tot 13 maanden afkappen</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Gebruik </p> </td> 
   <td colname="col2"> <p>Dit cookie wordt ingesteld door het domein van de klant nadat het AMCV-cookie door de client is ingesteld. Het doel van dit cookie is het permanent bijhouden van id's in de status van de eerste partij toe te staan en wordt als referentie-id gebruikt als het AMCV-cookie is verlopen. Kijk hier naar het AMCV-cookie voor meer informatie. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Locatie </p> </td> 
   <td colname="col2"> <p>Alleen CNAME-klanten. Niet van toepassing op scenario's van derden. Cookie wordt opgeslagen op uw domein, het zelfde domein dat door CNAME en uw het beeldverzoek van Analytics wordt gebruikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Grootte </p> </td> 
   <td colname="col2"> <p>45 bytes </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> SameSite=Lax </p> </td> 
   <td colname="col2"> <p>Cookies met deze instelling worden alleen verzonden wanneer het domein dat wordt weergegeven in de URL van de browser overeenkomt met het domein van de cookie. Deze instelling is de nieuwe standaardinstelling voor cookies in Chrome.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Naam cookie: AMCV_##@AdobeOrg**

De [ Dienst van identiteitskaart van Experience Platform ](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=nl-NL) gebruikt JavaScript om een unieke bezoekersidentiteitskaart in een `AMCV_###@AdobeOrg` koekje op het domein van de huidige website op te slaan, waar `###` een willekeurige koord van karakters, zoals `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.` vertegenwoordigt

Zie ook, [ Cookies en de Dienst van identiteitskaart ](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html?lang=nl-NL).

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Kenmerk </p> </th> 
   <th colname="col2" class="entry"> <p>Beschrijving </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p> Unieke bezoeker-id's die door Experience Cloud Solutions worden gebruikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Verlopen </p> </td> 
   <td colname="col2"> <p> 13 maanden </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Gebruik </p> </td> 
   <td colname="col2"> <p> Dit cookie wordt gebruikt om een unieke bezoeker te identificeren </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Locatie </p> </td> 
   <td colname="col2"> <p> Dit cookie wordt opgeslagen in het domein van de website (niet in het domein van de afbeeldingsaanvraag). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Grootte </p> </td> 
   <td colname="col2"> <p> De meeste klanten kunnen verwachten dat deze cookie ongeveer 200 bytes lang is. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Geen waarde toegevoegd. Chrome is standaard ingesteld op Lax. </p> </td> 
   <td colname="col2"> <p> Cookies met deze instelling worden alleen verzonden wanneer het domein dat wordt weergegeven in de URL van de browser overeenkomt met het domein van de cookie. Deze instelling is de nieuwe standaardinstelling voor cookies in Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
