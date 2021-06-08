---
description: Leer hoe de dienst van identiteitskaart wordt opgeslagen en gebruikt over Experience Cloud toepassingen.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target
title: 'Experience Cloud Cookies '
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Beheer
role: Administrator
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
source-git-commit: c7ed1324015beb7ebcf7a4ee21b05601e36e608f
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 2%

---

# Experience Cloud cookies{#experience-cloud-cookies}

Adobe Experience Cloud gebruikt cookies om een bezoeker-id op te slaan die in alle Experience Cloud-toepassingen wordt gebruikt.

**Naam cookie: s_ecid**

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
   <td colname="col2"> <p>2 jaar </p> </td> 
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

De [Experience Platform-id-service](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=en) gebruikt JavaScript om een unieke bezoeker-id op te slaan in een `AMCV_###@AdobeOrg`-cookie op het domein van de huidige website, waarbij `###` een willekeurige tekenreeks vertegenwoordigt, zoals `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.`

Zie ook [Cookies en de Dienst van identiteitskaart](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html?lang=en).

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
   <td colname="col2"> <p> Unieke bezoeker-id's die worden gebruikt door Experience Cloud Solutions. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Verlopen </p> </td> 
   <td colname="col2"> <p> 2 jaar </p> </td> 
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
   <td colname="col1"> <p>Geen waarde toegevoegd. Chrome wordt standaard ingesteld op Lax. </p> </td> 
   <td colname="col2"> <p> Cookies met deze instelling worden alleen verzonden wanneer het domein dat wordt weergegeven in de URL van de browser overeenkomt met het domein van de cookie. Deze instelling is de nieuwe standaardinstelling voor cookies in Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
