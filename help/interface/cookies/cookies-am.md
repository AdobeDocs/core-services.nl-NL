---
description: Meer informatie over Audience Manager cookies in Adobe Experience Cloud.
keywords: cookies
solution: Experience Cloud, Audience Manager
title: 'Audience Manager Cookies '
uuid: 8b384c38-b85a-4e93-b00e-41a9d3ae2b21
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 2%

---


# Audience Manager Cookies{#audience-manager-cookies}

Audience Manager vertrouwt op een paar eenvoudige koekjes om verschillende functies uit te voeren. Dit zijn onder andere het toewijzen van id&#39;s, het opnemen van gegevensaanroepen, het bijhouden van fouten en het testen om te controleren of cookies kunnen worden ingesteld. In deze sectie worden de verschillende cookies vermeld en beschreven die door de Audience Manager zijn ingesteld.

**demdex Cookie**

<table id="table_1CCF7EA2BC9E421F8DEECA5F611E33F6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Doel</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager </span> stelt dit cookie zo in dat een unieke id wordt toegewezen aan een sitebezoeker. Het <span class="wintitle"> demdex- </span> cookie helpt <span class="keyword"> Audience Manager basisfuncties uit te </span> voeren, zoals bezoekersidentificatie, id-synchronisatie, segmentatie, modellering, rapportage, enz. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhoud</b> </p> </td> 
   <td colname="col2"> <p>Het <span class="wintitle"> demdex- </span> cookie bevat een unieke gebruikersnaam (UUID), zoals in het onderstaande voorbeeld wordt getoond: </p> <p> <span class="codeph"> 06151304227769720433039235178204449977 </span> </p> <p>See also, <a href="https://docs.adobe.com/content/help/en/audience-manager/user-guide/reference/ids-in-aam.html" format="https" scope="external"> Index of IDs in Audience Manager </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Overige kenmerken</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_11291DA87C5045E880034E06C863BCDA"> 
      <li id="li_40C30A06A12449A4A8748621223CA71B">Levensduur: Het <span class="wintitle"> demdex- </span> cookie heeft een time-to-live (TTL) interval van 180 dagen. De TTL wordt teruggesteld aan 180 dagen op elke gebruikersinteractie met een partnerwebsite. Het cookie verloopt als een gebruiker niet binnen het TTL-interval terug naar uw site komt. </li> 
      <li id="li_A589EDA2198249829207A183872EF1FF">Uitschakelen: <span class="keyword"> Audience Manager </span> herstelt de cookie met een <span class="codeph"> Do Not Adobe Target </span> -tekenreeks als een gebruiker de gegevensverzameling uitschakelt. In dit geval wordt de cookie-TTL ingesteld op 10 jaar. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**dextp Cookie**

<table id="table_7343C9C9ADD24D3FA693ECC76E4A4045"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Doel</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager </span> plaatst dit koekje om de laatste tijd te registreren het een vraag van de gegevenssynchronisatie maakte. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhoud</b> </p> </td> 
   <td colname="col2"> <p>Het <span class="wintitle"> dextp- </span> cookie bevat een naam of id van een gegevensaanbieder en een UNIX UTC-tijdstempel die is opgemaakt als door pipe gescheiden tekenreeksen. In the examples, <i>italics</i> represents a variable placeholder. </p> <p> 
     <ul id="ul_80D0BC3FCF06470991E12712401D784A"> 
      <li id="li_03747A433CEB4756A26CD866E716B89D">Oude stijl: <span class="codeph"> <span class="varname"> naam van de gegevensaanbieder hier </span>-1490307822097| <span class="varname"> naam van de gegevensaanbieder hier </span>-1490307822038 </span> </li> 
      <li id="li_79E7000E82DB4ADA9E9887B017343B2D">Nieuwe stijl: <span class="codeph"> 21-1-1490307821616|544-1-1490307821793|3-1-1490307821852|42 0-1-1490307822038| </span> </li> 
     </ul> </p> <p>Zie ook de onderstaande sectie over de syntaxis van dextp-gegevens. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Overige kenmerken</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4922AC2CD55D4C888A6FBEB22F8B889B"> 
      <li id="li_91A68C44E53840379C2ACDED25468735">Levensduur: Het <span class="wintitle"> dextp- </span> cookie heeft een time-to-live (TTL) interval van 180 dagen. </li> 
      <li id="li_6B8C674EFAAC4DABA0A640CF29247F99">Uitschakelen: <span class="keyword"> Audience Manager </span> herstelt de cookie met een <span class="codeph"> Do Not Adobe Target </span> -tekenreeks als een gebruiker de gegevensverzameling uitschakelt. In dit geval wordt de cookie-TTL ingesteld op 10 jaar. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Syntaxis gegevens dextp Cookie:

De volgende tabel bevat een lijst met en definieert de elementen in een cookie op locatie in de gegevenstekenreeks. [!DNL dextp]

<table id="table_BE00604B97F24F5A94AA4F566063D785"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Positie variabele </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Eerste of tweede</b> </p> </td> 
   <td colname="col2"> <p>De positie van de naam of id van de gegevensaanbieder hangt af van de vraag of de cookie de nieuwe of oude opmaak gebruikt. </p> <p> <b>Opmaak van oude stijl:</b> </p> <p> 
     <ul id="ul_5BFBF40E3FE849CA859030F2D070FDF6"> 
      <li id="li_E8F4DC0CB15B472ABE9892B3A61D7F77">Syntaxis: <span class="codeph"> <span class="varname"> naam gegevensaanbieder </span> <span class="varname"> - UNIX UTC-tijdstempel </span> </span> </li> 
      <li id="li_7CD8B101156140F49EA97B18E9591402">Voorbeeld: <span class="codeph"> dataProvider1 - 1490307822038 </span> </li> 
     </ul> </p> <p>De cookie van de oude stijl identificeert de gegevensaanbieder met een leesbare naam. </p> <p> <b>Nieuwe stijlopmaak:</b> </p> <p> 
     <ul id="ul_AC6225CA781746148C125F21DFED1ED9"> 
      <li id="li_29C4B52E398B4EA28944980A15B05A57">Syntaxis: <span class="codeph"> <span class="varname"> gegevensleverancier-id </span> - 1|2 - <span class="varname"> UNIX UTC-tijdstempel </span> </span> </li> 
      <li id="li_3BF30CA5FED242DF96E0B54AFC64B06F">Voorbeeld: <span class="codeph"> 123345 - 1 - 1490307822038 </span> </li> 
     </ul> </p> <p>De nieuwe stijlcookie: </p> <p> 
     <ul id="ul_F05A91A455FA44C7A71186C0C9E31630"> 
      <li id="li_A8C9638173684359BABC4207845A4F48">Hiermee wordt de naam van de leesbare gegevensaanbieder vervangen door een numerieke id. </li> 
      <li id="li_28F1E2DB24904E53BE9718AD788CE61E">Identificeert het vraagtype met identiteitskaart 1 of identiteitskaart 2. ID 1 vertegenwoordigt een de synchronisatievraag van identiteitskaart. ID 2 vertegenwoordigt een afgekeurde vraag die niet meer wordt gebruikt. U mag niet veel (of enige) dextp-cookies met ID 2 zien. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Laatste</b> </p> </td> 
   <td colname="col2"> <p>De laatste positie bevat een UNIX UTC-tijdstempel. </p> </td> 
  </tr> 
 </tbody> 
</table>

**dst Cookie**

<table id="table_83AE9B6350C6408BAECD9FCF33022B98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Doel</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager </span> stelt dit cookie in wanneer er een fout optreedt bij het verzenden van gegevens naar een <a href="https://docs.adobe.com/content/help/en/audience-manager/user-guide/features/destinations/destinations.html#purposes" format="https" scope="external"> doel </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhoud</b> </p> </td> 
   <td colname="col2"> <p> Het <span class="wintitle"> DST- </span> cookie bevat sets met doel-id's en UNIX-tijdstempels die zijn opgemaakt als door pipe gescheiden tekenreeksen. In the examples, <i>italics</i> represents a variable placeholder. </p> <p> 
     <ul id="ul_CE98076A02DA413486C1D341E9806889"> 
      <li id="li_850209D956644749B98C7A208C825C15">Syntaxis: <span class="codeph"> <span class="varname"> doel-id </span> - <span class="varname"> UNIX UTC-tijdstempel </span> </span> </li> 
      <li id="li_4A22152C70844733982230EBF7B9EB78">Voorbeeld: <span class="codeph"> 067797-1490349684|1010788-1490349692|1067797-149034962 </span> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Overige kenmerken</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_5D13DD701B484B51BF2808A69A919106"> 
      <li id="li_4E665114C63246FBA32A4E19984D2693">Levensduur: Het <span class="wintitle"> dst- </span> cookie heeft een time-to-live (TTL) interval van 180 dagen. </li> 
      <li id="li_A682B566704F43D2AB72487EFF212474">Uitschakelen: <span class="keyword"> Audience Manager </span> herstelt de cookie met een <span class="codeph"> Do Not Adobe Target </span> -tekenreeks als een gebruiker de gegevensverzameling uitschakelt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**_dp Cookie**

Dit is een tijdelijke cookie. [!DNL Audience Manager] probeert om het [!DNL _dp] koekje te plaatsen om te bepalen of het andere koekjes in het demdex.net domein in een derdecontext kan plaatsen. Wanneer [!DNL _dp] deze is ingesteld, bevat deze de waarde 1. [!DNL Audience Manager] leest deze waarde en verwijdert het cookie onmiddellijk. Als het [!DNL _dp] cookie niet aanwezig is, [!DNL Audience Manager] weet het dat het geen cookies kan instellen.