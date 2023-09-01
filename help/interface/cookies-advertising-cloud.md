---
description: Leer meer over Adobe Advertising cookies voor het toewijzen en plaatsen van afspraken aan conversiegebeurtenissen en, mogelijk, het gebruik van die informatie voor het optimaliseren van advertenties.
title: Cookies Adoben Advertising
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: 5d0e02713ec4b233e06ecd3ac0234d1526b947f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 4%

---

# Cookies Adoben Advertising{#advertising-cloud-cookies}

Adobe Advertising (voorheen Adobe Advertising Cloud) gebruikt cookies om gebeurtenissen voor conversie in kaart te brengen en te koppelen aan conversiegebeurtenissen en deze informatie mogelijk te gebruiken om advertenties te optimaliseren.

>[!NOTE]
>
>De JavaScript-tag voor bètaAdoben Advertising die de tag [Adobe Experience Cloud ID-service (ECID)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) create [Experience Cloud_ecid-cookies van eerste fabrikant](cookies-first-party.md), niet Adobe Advertising cookies.

## Naam cookie: _lcc

<table id="table_821F8EBE91F244CBA72B0975B961B908"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>Id's en tijdstempels (in de notatie jjjjjjjjjjjjjjmmdd) van weergave klikken</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>15 minuten</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een cookie van een andere fabrikant die wordt gebruikt om te bepalen of een klikgebeurtenis op een display wordt toegepast en op een Adobe Analytics-hit wordt toegepast </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>52 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: _tag

<table id="table_28C2B62595E240D5A3C3E0BE147748C1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>Gecodeerde id's en tijdstempels voor advertentiegerelateerde services met behulp van Adobe Advertising DSP-tracking </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>1 jaar </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een cookie van een andere fabrikant die gebruikersrelaties opslaat met advertenties, zoals "last seen ad xyz123 on June 30, 2016" </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>Variabele; gegevens worden gecodeerd en doorgaans minder dan 1 kB </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: adcloud

<table id="table_D7CD238736BC4571883F92F47673F57C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>De tijdstempels van het laatste bezoek van de surfer aan de website van de adverteerder en de laatste zoekklik van de surfer, en de ef_id die werd gemaakt toen de gebruiker op een advertentie klikte</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>1 jaar</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een eersteklas cookie die de surfer-id koppelt aan relevante publiekssegmenten en conversies </p> <p> Informatie over het laatste bezoek wordt gebruikt om de laadtijden van de pagina te optimaliseren door onnodige verzoeken om [!DNL Adobe] servers. </p> <p>Met informatie over de laatste zoekklik kunt u bepalen of een conversiegebeurtenis het resultaat is van een klik of een doorkijkbewerking (conversie als gevolg van indrukkingen maar zonder klikken). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>Het topdomein van de adverteerder (bijvoorbeeld example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>Variabele, maar doorgaans 50-150 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: ev_sync_&#42;

(ev_sync_ax, ev_sync_bk, ev_sync_dd, ev_sync_fs, ev_sync_nx, ev_sync_ox, ev_sync_pm, ev_sync_rc, ev_sync_tm, ev_sync_yh)

<table id="table_A05C02AB261946E0AABAD78259392D81"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>De datum waarop de synchronisatie wordt uitgevoerd, in de notatie jjjjjjjjjjmmdd </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>De datum waarop de synchronisatie wordt uitgevoerd, in de notatie jjjjjjjjjjmmdd </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een derde partij, en ruilspecifieke koekje dat de Adobe Advertising overfer identiteitskaart met de partner en de uitwisseling synchroniseert. Het is gecreeerd voor nieuwe surfers en verzendt een synchronisatieverzoek wanneer het is verlopen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>8 tekens </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: everest_g_v2

<table id="table_04043292A43B41B69EAF17AF4E217C69"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>De browser en de surfer-id </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>1 jaar </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Gemaakt nadat een gebruiker eerst op de advertentie van een klant klikt en vervolgens de huidige en volgende muisklik op de website van de client heeft toegewezen </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>~27 tekens </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: everest_session_v2

<table id="table_1A3AE4CA71304ADB943CB1F64BE695F5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>De sessie-id </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>Wanneer de browser wordt gesloten </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een browsersessiecookie van derden; één cookie wordt gebruikt voor alle accounts </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>~16 tekens </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: ev_tm

<table id="table_6C4D9DCFA4BF4FB2BD445E027550955F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>Adobe Advertising DSP (Demand Side Platform)-id </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>2 jaar </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Een cookie van een andere fabrikant die de DSP-id opslaat die overeenkomt met de surfer-id in het cookie everest_g_v2 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>~20 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Naam cookie: id_adcloud

<table> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Opgeslagen informatie </p> </td> 
   <td colname="col2"> <p>De surfer-id </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verlopen </p> </td> 
   <td colname="col2"> <p>91 dagen </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gebruik </p> </td> 
   <td colname="col2"> <p>Het cookie wordt ingesteld in het domein van de eerste gebruiker, maar wordt nog niet gebruikt </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Locatie </p> </td> 
   <td colname="col2"> <p>Het topdomein van de adverteerder (bijvoorbeeld example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Grootte </p> </td> 
   <td colname="col2"> <p>16 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>
