---
description: Meer informatie over gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar Experience Cloud.
keywords: Klantkenmerken;kernservices
solution: Experience Cloud
title: 'Meer informatie over gegevensbestanden en gegevensbronnen voor klantkenmerken '
uuid: 9dd0e364-889b-45db-b190-85c0930a101e
feature: Klantkenmerken
topic: Beheer
role: Admin
level: Experienced
exl-id: e2dfe10d-7003-4afa-a5e6-57703d74efd4
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '1187'
ht-degree: 0%

---

# Gegevensbestand en gegevensbronnen voor klantkenmerken

Gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar Experience Cloud.

U hebt toegang tot CRM of vergelijkbare gegevens van uw onderneming nodig. De gegevens die u uploadt naar de Experience Cloud moeten een `.csv` bestand zijn. Als u uploadt via FTP of sFTP, uploadt u ook een `.fin` dossier.

Kenmerken van klanten zijn ontworpen om enkele bestanden per dag af te handelen. Om de kwestie te verlichten van het hebben van vele kleine dossiers vertragend verwerking, worden de dossiers die binnen 30 minuten van een vorige partij van de zelfde organisatie worden verzonden verpletterd aan een laag-prioritaire rij.

## Toegestane bestandstypen en vereisten voor naamgeving {#section_6F64FA02ACCC4215B0862CB6A1821FBF}

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Bestandstype </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv  </span> </p> </td> 
   <td colname="col2"> <p>Een bestand met door komma's gescheiden waarden (bijvoorbeeld een bestand dat in Excel is gemaakt). Dit bestand bevat de kenmerkgegevens van de klant. </p> <p> <b>Naamgevingsvereisten:</b> zorg ervoor dat bestandsextensies geen witruimten bevatten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin  </span> </p> </td> 
   <td colname="col2"> <p>(Vereist) Het <span class="filepath"> .fin </span> dossier vertelt het systeem dat u klaar bent met het uploaden van gegevens. De naam van het <span class="filepath"> .fin </span> bestand moet overeenkomen met de naam van het <span class="filepath"> .csv </span> bestand. </p> <p>Adobe raadt u aan een leeg tekstbestand met de extensie <span class="filepath"> .fin </span> te maken. Een leeg bestand bespaart ruimte en uploadt tijd. </p> <p> <p>Opmerking:  Het is niet toegestaan de naam van een <span class="filepath"> .fin </span>-bestand te wijzigen nadat het is geüpload. Het <span class="filepath"> .fin </span>-bestand moet afzonderlijk worden geüpload en kan geen hernoemd, eerder geüpload bestand zijn. </p> </p> <p>Nadat u het <span class="filepath"> .fin </span> dossier in de FTP van de Attributen van de Klant uploadt, wint het systeem snel (binnen één minuut) gegevens terug. Dit verschilt van andere Adobe FTP-gebaseerde systemen, die gegevens minder vaak (ongeveer één keer per uur) ophalen. </p> <p>Het <span class="filepath"> .fin </span> dossier wordt niet vereist wanneer het gebruiken van de belemmering-en-dalings uploadmethode. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz  </span> of  <span class="filepath"> .zip  </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz  </span> (gzip) of  <span class="filepath"> .zip  </span> - voor gecomprimeerde bestanden. Een ZIP-bestand <span class="filepath"> .zip </span> kan niet meer dan één bestand in het archief bevatten. </p> <p> <b>Naamgevingsvereisten:</b> de naam van het bestand  <span class="filepath"> .zip  </span> of  <span class="filepath"> .gz  </span> moet overeenkomen met de naam van het bestand  <span class="filepath"> .csv  </span>. Als uw <span class="filepath"> .csv </span>-bestand bijvoorbeeld <span class="filepath"> crm_small.csv </span> is, moet het ZIP <span class="filepath"> .zip </span>-bestand <span class="filepath"> crm_small.csv.zip </span> zijn. </p> <p>Het .fin- dossier moet .csv aanpassen. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Vereisten voor de kenmerkgegevensbestanden {#section_169FBF5B7BBA47CE825B7A330CF3FE98}

**Voorbeeld-CSV**

Het CSV-bestand moet de volgende indeling hebben:

![](assets/cvs.png)

Hetzelfde bestand wordt weergegeven in een teksteditor:

![](assets/csv_txt.png)

**Richtsnoeren**

<table id="table_A9849CC9AA784763921DE057F0F61515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Item </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Slepen en neerzetten </p> </td> 
   <td colname="col2"> <p>Het bestand voor slepen en neerzetten moet kleiner zijn dan 100 MB. </p> <p>Het <span class="filepath"> .fin </span> dossier wordt niet vereist wanneer het gebruiken van de belemmering-en-dalings uploadmethode. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kolom Klant-id </p> </td> 
   <td colname="col2"> <p> De eerste kolom moet een unieke klant-id zijn. Gebruikte identiteitskaart zou aan identiteitskaart moeten beantwoorden die aan de Dienst van identiteitskaart van de Experience Cloud wordt overgegaan. </p> <p>Voor Analytics wordt de id opgeslagen in een proxy of eVar. </p> <p>Voor Target, de waarde setCustomerID. (Zie <a href="core-services.md#section_AD473A6A21C1446498E700363F9A8437" format="dita" scope="local"> Analytics &amp; Adobe Target - synchroniseert de klant-id </a>) </p> <p> Deze klant-id is de unieke id die uw CRM gebruikt voor elke persoon in uw database. De resterende kolommen zijn attributen die uit uw CRM komen. U kiest hoeveel kenmerken u wilt uploaden. </p> <p>U kunt goed leesbare namen aanbevelen voor de kolomkoppen, maar deze zijn niet vereist. Wanneer u het schema na het uploaden valideert, kunt u vriendelijke namen toewijzen aan de geüploade rijen en kolommen. </p> <p> <b>Informatie over Customer ID's</b> </p> <p>Een onderneming gebruikt doorgaans een klant-id van een CRM-systeem. Deze id wordt ingesteld met behulp van de <span class="codeph"> setCustomerIDs </span>-oproep wanneer een persoon zich aanmeldt. Deze id wordt ook gebruikt als de sleutel in het CRM-bestand dat naar de Experience Cloud wordt geüpload. Een <a href="t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8" format="dita" scope="local"> Alias-id </a> is een vriendelijke naam voor een gegevensopslag in Audience Manager, waar de aliasgegevens worden opgeslagen. Het systeem verzendt aliassen naar deze gegevensopslag (via setCustomerIDs). Het CRM-bestand wordt toegepast op de gegevens in die gegevensopslag. </p> <p>Voor <span class="codeph"> setCustomerIDs </span> informatie, zie <a href="https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=en" format="https" scope="external"> Klant IDs en de Status van de Authentificatie </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Volgende koppen en kolommen </p> </td> 
   <td colname="col2"> <p>De volgende kopballen zouden de naam van elk attribuut moeten vertegenwoordigen. </p> <p> Deze kolommen zouden de Attributen van de Klant moeten bevatten die uit CRM komen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kenmerklimieten </p> </td> 
   <td colname="col2"> <p>U kunt honderden <span class="filepath"> .csv </span> kolommen aan de dienst van de Attributen van de Klant in de Experience Cloud uploaden. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten, afhankelijk van de oplossingen die u hebt: </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analysestandaard</b>: 3 totaal </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 200 per rapportsuite </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Adobe Target Standard:</b> 5 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b>Adobe Target Premium:</b> 200 </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Rijlimieten </p> </td> 
   <td colname="col2"> <p>Er is geen limiet voor het aantal rijen bekend. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kolomlimieten </p> </td> 
   <td colname="col2"> <p>Voor de uitvoerbaarheid beperkt u het aantal kolommen tot ongeveer 200. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tekenbeperkingen </p> </td> 
   <td colname="col2"> <p>Als u een abonnement op Analytics maakt, wordt de veldlengte voor de geüploade bestanden afgebroken tot 255. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>FTP-richtlijnen en groottebeperkingen </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_E157EE6F98914EADA0C103D1D1E705D3"> 
      <li id="li_84FBD455DD164A28AC16F4A5AB19E4B3">Maximale bestandsgrootte voor FTP is 4 GB voor elke upload. </li> 
      <li>Minimale bestandsgroottelimiet voor 10 MB voor elke upload. </li>
      <li>U kunt elk half uur één bestand uploaden. </li>
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> Plaats het .csv-bestand <span class="filepath"> (en <span class="filepath"> .fin </span>) in de hoofdmap van de FTP-site.</span> </li> 
     </ul> </p> <p> <p>Belangrijk:  De totale toegestane ruimte voor de FTP-account is 40 GB. Het is uw verantwoordelijkheid om verwerkte bestanden te verwijderen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bestandsvereisten </p> </td> 
   <td colname="col2"> <p> Elke kenmerkbron moet hetzelfde aantal door komma's gescheiden velden bevatten. </p> <p> Velden met een regeleinde, een dubbel aanhalingsteken of komma moeten worden opgegeven. </p> <p> Dubbele aanhalingstekens in een veld moeten worden voorkomen met een backslash (\). </p> <p> Lege kolommen worden opgeslagen als <span class="term"> null </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Meerdere bestanden </p> </td> 
   <td colname="col2"> <p>Wanneer u kenmerkgegevens van de klant uploadt en u meerdere bestanden hebt die u snel na elkaar wilt uploaden, en vooral als de bestanden groot zijn, moet u controleren of het vorige bestand is verwerkt voordat u het volgende bestand uploadt. U kunt dit controleren door te controleren wanneer het vorige bestand is verplaatst naar de verwerkte of mislukte map in uw [!UICONTROL Customer Attributes] FTP-account. </p> <p> Wanneer u een groot bestand in kleinere bestanden splitst en snel na elkaar verzendt, kan dit de verwerking vertragen, tenzij u ervoor kunt zorgen dat elk bestand wordt verwerkt voordat het volgende bestand wordt verzonden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tekencodering </p> </td> 
   <td colname="col2"> <p>Voor Japan is UTF-8 verplicht. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>Historische gegevens </p> </td> 
   <td colname="col2"> <p> Klantkenmerken zijn gekoppeld aan het onderliggende bezoekersprofiel in [!DNL Analytics]. Als zodanig is [!UICONTROL Customer Attributes] gedurende de gehele levensduur van dat bezoekersprofiel gekoppeld aan de bezoeker in [!DNL Analytics]. Dit profiel bevat gedrag dat is opgetreden voordat de klant zich voor het eerst heeft aangemeld. </p> <p> Als u de backfill methode van de Data Warehouse gebruikt, zijn de gegevens gebonden aan post_visid_high/low die op analytics ID (HULP) gebaseerd is. Als u de dienst van identiteitskaart van de Experience Cloud gebruikt, zijn de gegevens gebonden aan post_visid_high/low die op Experience Cloud identiteitskaart (MID) gebaseerd is. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gegevensfeeds </p> </td> 
   <td colname="col2"> <p>Kenmerken van de klant zijn niet beschikbaar in gegevensfeeds. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Meerdere gegevensbronnen gebruiken {#section_76DEB6001C614F4DB8BCC3E5D05088CB}

Wanneer het creëren van, het wijzigen van, of het schrappen van de bronnen van de Attributen van de Klant, is er een vertraging rond één uur alvorens IDs met de nieuwe gegevensbron begint te synchroniseren.

De alias-id voor elke kenmerkbron van de klant moet uniek zijn. Als u meerdere gegevensbronnen hebt die dezelfde id gebruiken, kunnen deze als volgt worden ingesteld:

**In VisitorAPI.js of het gereedschap Experience Cloud-id in dynamisch tagbeheer:**

Stel twee klant-id&#39;s in die overeenkomen met de juiste gegevensbronnen:

```
Visitor.setCustomerIDs({ 
     "ds_id1”:"123456", 
     "ds_id2":"123456" 
});
```

(Zie [Klantnamen en verificatiestatus](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=en) voor meer informatie.)

In **[!UICONTROL Experience Cloud]** > **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**:

Maak twee bronnen voor klantkenmerken met behulp van unieke alias-id&#39;s die overeenkomen met de bovenstaande klant-id&#39;s. Met deze methode kan dezelfde referentie-id naar meerdere bronnen van kenmerk van klant worden verzonden.
