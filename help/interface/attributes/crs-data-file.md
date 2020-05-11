---
description: Gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar de Experience Cloud.
keywords: Customer Attributes;core services
seo-description: Gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar de Experience Cloud.
seo-title: Gegevensbestand en gegevensbronnen voor klantkenmerken
solution: Experience Cloud
title: Gegevensbestand en gegevensbronnen voor klantkenmerken
uuid: 9dd0e364-889b-45db-b190-85c0930a101e
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---


# Gegevensbestand en gegevensbronnen voor klantkenmerken

Gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar de Experience Cloud.

U zult toegang tot CRM of gelijkaardige gegevens van uw onderneming nodig hebben. De gegevens die u uploadt naar de Experience Cloud moeten een `.csv` bestand zijn. Als u uploadt via FTP of sFTP, uploadt u ook een `.fin` bestand.

Kenmerken van klanten zijn ontworpen om enkele bestanden per dag af te handelen. Om de kwestie te verlichten van het hebben van een groot aantal kleine dossiers vertragend verwerking, worden de dossiers die binnen 30 minuten van een vorige partij van de zelfde organisatie worden verzonden verpletterd aan een laag-prioritaire rij.

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
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>Een bestand met door komma's gescheiden waarden (bijvoorbeeld een bestand dat in Excel is gemaakt). Dit is het dossier dat de gegevens van het klantenattribuut bevat. </p> <p> <b>Naamgevingsvereisten:</b> Zorg ervoor dat bestandsextensies geen witruimten bevatten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Vereist) Het <span class="filepath"> .fin- </span> bestand geeft aan dat u klaar bent met het uploaden van gegevens. De naam van het <span class="filepath"> .fin- </span> bestand moet overeenkomen met de naam van het <span class="filepath"> .csv- </span> bestand. </p> <p>Adobe raadt u aan een leeg tekstbestand met de <span class="filepath"> extensie .fin te maken </span> . Een leeg bestand bespaart ruimte en uploadt tijd. </p> <p> <p>Opmerking:  De naam van een <span class="filepath"> .fin- </span> bestand mag niet worden gewijzigd nadat het is geüpload. Het <span class="filepath"> .fin- </span> bestand moet afzonderlijk worden geüpload en kan geen hernoemd, eerder geüpload bestand zijn. </p> </p> <p>Nadat u het <span class="filepath"> .fin- </span> bestand in de FTP van de Attributen van de Klant uploadt, wint het systeem snel (binnen één minuut) gegevens terug. Dit verschilt van andere op FTP gebaseerde systemen van Adobe, die gegevens minder vaak (ongeveer één keer per uur) opvangen. </p> <p>Het <span class="filepath"> .fin- </span> bestand is niet vereist wanneer u de uploadmethode voor slepen en neerzetten gebruikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz </span> of <span class="filepath"> .zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz </span> (gzip) of <span class="filepath"> .zip </span> - voor gecomprimeerde bestanden. Een <span class="filepath"> .zip- </span> bestand mag niet meer dan één bestand in het archief bevatten. </p> <p> <b>Naamgevingsvereisten:</b> De naam van het <span class="filepath"> .zip- </span> of <span class="filepath"> .gz-bestand </span> moet overeenkomen met de naam van het <span class="filepath"> .csv-bestand </span>. Als uw <span class="filepath"> .csv- </span> bestand bijvoorbeeld <span class="filepath"> crm_small.csv is </span>, moet het <span class="filepath"> .zip- </span> bestand <span class="filepath"> crm_small.csv.zip zijn </span>. </p> <p>Het .fin- dossier moet .csv aanpassen. </p> </td> 
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
   <td colname="col2"> <p>Het bestand voor slepen en neerzetten moet kleiner zijn dan 100 megabytes. </p> <p>Het <span class="filepath"> .fin- </span> bestand is niet vereist wanneer u de uploadmethode voor slepen en neerzetten gebruikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kolom Klant-id </p> </td> 
   <td colname="col2"> <p> De eerste kolom moet een unieke klant-id zijn. De gebruikte id moet overeenkomen met de id die wordt doorgegeven aan de Experience Cloud ID Service. </p> <p>Voor Analytics wordt de id opgeslagen in een prop of eVar. </p> <p>Voor Target, de waarde setCustomerID. (Zie <a href="../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437" format="dita" scope="local"> Analytics &amp; Adobe Target - de klant-id synchroniseren </a>) </p> <p> Deze klant-id is de unieke id die uw CRM gebruikt voor elke persoon in uw database. De resterende kolommen zijn attributen die uit uw CRM komen. U bepaalt hoeveel kenmerken u wilt uploaden. </p> <p>U kunt goed leesbare namen aanbevelen voor de kolomkoppen, maar deze zijn niet vereist. Wanneer u het schema na het uploaden valideert, kunt u vriendelijke namen toewijzen aan de geüploade rijen en kolommen. </p> <p> <b>Informatie over Customer ID's</b> </p> <p>Een onderneming gebruikt doorgaans een klant-id van een CRM-systeem. Deze id wordt ingesteld met de <span class="codeph"> </span> aanroep van setCustomerID's wanneer een persoon zich aanmeldt. Deze id wordt ook gebruikt als de sleutel in het CRM-bestand dat naar de Experience Cloud wordt geüpload. Een <a href="../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8" format="dita" scope="local"> alias-id </a> is een vriendelijke naam voor een gegevensopslag in Audience Manager, waar de aliasgegevens worden opgeslagen. Het systeem verzendt aliassen naar deze gegevensopslag (via setCustomerIDs). Het CRM-bestand wordt toegepast op de gegevens in die gegevensopslag. </p> <p>Voor <span class="codeph"> setCustomerIDs- </span> informatie, zie <a href="https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html" format="https" scope="external"> Klant IDs en de Staat van de Authentificatie </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Volgende koppen en kolommen </p> </td> 
   <td colname="col2"> <p>De volgende kopballen zouden de naam van elk attribuut moeten vertegenwoordigen. </p> <p> Deze kolommen zouden de Attributen van de Klant moeten bevatten die uit CRM komen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kenmerklimieten </p> </td> 
   <td colname="col2"> <p>U kunt honderden <span class="filepath"> .csv- </span> kolommen uploaden naar de klantenkenmerkservice in de Experience Cloud. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten, afhankelijk van de oplossingen die u hebt: </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analysestandaard</b>: 3 totaal </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 200 per rapportsuite </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Adobe Target-standaard:</b> 5 </li> 
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
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> U moet het <span class="filepath"> .csv-bestand </span> (en <span class="filepath"> .fin-bestand </span>) in de hoofdmap van de FTP-site plaatsen. </li> 
     </ul> </p> <p> <p>Belangrijk:  De totale toegestane ruimte voor de FTP-account is 40 GB. Het is uw verantwoordelijkheid om verwerkte bestanden te verwijderen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bestandsvereisten </p> </td> 
   <td colname="col2"> <p> Elke kenmerkbron moet hetzelfde aantal door komma's gescheiden velden bevatten. </p> <p> Velden met een regeleinde, een dubbel aanhalingsteken of komma moeten worden opgegeven. </p> <p> Dubbele aanhalingstekens in een veld moeten worden voorkomen met een backslash (\). </p> <p> Lege kolommen worden opgeslagen als <span class="term"> null </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Meerdere bestanden </p> </td> 
   <td colname="col2"> <p>Als u kenmerkgegevens van klanten uploadt en u meerdere bestanden hebt die u snel na elkaar wilt uploaden, en vooral als de bestanden groot zijn, moet u controleren of het vorige bestand is verwerkt voordat u het volgende bestand uploadt. U kunt dit controleren door te controleren wanneer het vorige bestand is verplaatst naar de verwerkte of mislukte map in uw FTP-account met klantkenmerken. </p> <p> Wanneer u een groot bestand in kleinere bestanden splitst en snel na elkaar verzendt, kan dit de verwerking vertragen, tenzij u ervoor kunt zorgen dat elk bestand volledig wordt verwerkt voordat het volgende wordt verzonden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tekencodering </p> </td> 
   <td colname="col2"> <p>Voor Japan is UTF-8 verplicht. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>Historische gegevens </p> </td> 
   <td colname="col2"> <p> Kenmerken van de klant zijn gekoppeld aan het onderliggende bezoekersprofiel in Analytics. De klantkenmerken zijn daarom gekoppeld aan de bezoeker gedurende de gehele levensduur van dat bezoekersprofiel in Analytics. Dit omvat gedrag dat voorkwam alvorens de klant voor het eerst het programma opende. </p> <p> Als u de backfill methode van het gegevenspakhuis gebruikt, zijn de gegevens gebonden aan post_visid_high/low die op analytische identiteitskaart (HULP) gebaseerd is. Als u de Experience Cloud ID Service gebruikt, zijn de gegevens gekoppeld aan een post_visid_high/low die is gebaseerd op Experience Cloud ID (MID). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gegevensfeeds </p> </td> 
   <td colname="col2"> <p>Kenmerken van de klant zijn niet beschikbaar in gegevensfeeds. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Meerdere gegevensbronnen gebruiken {#section_76DEB6001C614F4DB8BCC3E5D05088CB}

Wanneer het creëren van, het wijzigen van, of het schrappen van de bronnen van de klantenattributen, is er een vertraging rond één uur alvorens IDs met de nieuwe gegevensbron begint te synchroniseren.

Alias ID voor elke bron van klantkenmerken moet uniek zijn. Als u meerdere gegevensbronnen hebt die dezelfde id gebruiken, moeten deze als volgt worden ingesteld:

**In VisitorAPI.js of het hulpmiddel van de identiteitskaart van de Ervaring Cloud in dynamisch markeringsbeheer:**

Stel twee klant-id&#39;s in die overeenkomen met de juiste gegevensbronnen:

```
Visitor.setCustomerIDs({ 
     "ds_id1”:"123456", 
     "ds_id2":"123456" 
});
```

(Zie ID&#39;s van [klanten en verificatiestatus](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) voor meer informatie.)

In het **[!UICONTROL Experience Cloud]** > **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**:

Maak twee bronnen voor klantkenmerken met behulp van unieke alias-id&#39;s die overeenkomen met de bovenstaande klant-id&#39;s. Met deze methode kan dezelfde referentie-id naar meerdere bronnen voor klantkenmerken worden verzonden.
