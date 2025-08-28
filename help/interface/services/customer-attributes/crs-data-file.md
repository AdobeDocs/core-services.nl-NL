---
description: Meer informatie over gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerken naar Experience Cloud.
solution: Experience Cloud
title: Gegevensbestand en gegevensbronnen
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: e2dfe10d-7003-4afa-a5e6-57703d74efd4
source-git-commit: 106ad989c5eef60dabbe4b82deaed9d87b09d795
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 0%

---

# Gegevensbestand en gegevensbronnen voor [!DNL Customer Attributes]

Gegevensbestandsvereisten en meerdere gegevensbronnen voor het uploaden van klantkenmerkgegevens naar Experience Cloud.

U hebt toegang tot CRM of vergelijkbare gegevens van uw onderneming nodig. De gegevens die u uploadt naar Experience Cloud, moeten een `.csv` -bestand zijn. Als u uploadt via FTP of sFTP, uploadt u ook een `.fin` bestand.

[!DNL Customer Attributes] is ontworpen om enkele bestanden per dag af te handelen. Om de kwestie te verlichten van het hebben van vele kleine dossiers vertragend verwerking, worden de dossiers die binnen 30 minuten van een vorige partij van de zelfde organisatie worden verzonden verpletterd aan een laag-prioritaire rij.

## Toegestane bestandstypen en vereisten voor naamgeving {#section_6F64FA02ACCC4215B0862CB6A1821FBF}

| Bestandstype | Beschrijving |
|--- |--- |
| `.csv` | Een bestand met door komma&#39;s gescheiden waarden (bijvoorbeeld een bestand dat in Excel is gemaakt). Dit bestand bevat de klantkenmerkgegevens.   Naamgevingsvereisten: zorg ervoor dat bestandsextensies geen witruimten bevatten. |
| `.fin` | (Vereist) Het `.fin` -bestand geeft aan het systeem door dat u klaar bent met het uploaden van gegevens. De naam van het bestand `.fin` moet overeenkomen met de naam van het bestand `.csv` .  Adobe raadt u aan een leeg tekstbestand met de extensie `.fin` te maken. Een leeg bestand bespaart ruimte en uploadt tijd. **Nota:** het anders noemen van een `.fin` dossier wordt niet toegestaan nadat het wordt geupload. Het `.fin` -bestand moet afzonderlijk worden geüpload en kan geen hernoemd, eerder geüpload bestand zijn. Nadat u het `.fin` -bestand in de attributen FTP van de klant hebt geüpload, haalt het systeem snel gegevens op (binnen één minuut). Dit verschilt van andere op FTP gebaseerde Adobe-systemen, die gegevens minder vaak (ongeveer één keer per uur) ophalen. Het bestand `.fin` is niet vereist wanneer u de uploadmethode voor slepen en neerzetten gebruikt. |
| `.gz` of `.zip` | `.gz` (gzip) of `.zip` - voor gecomprimeerde bestanden. Een `.zip` -bestand mag niet meer dan één bestand in het archief bevatten. Naamgevingsvereisten: de naam van het bestand `.zip` of `.gz` moet overeenkomen met de naam van het bestand `.csv` . Als uw `.csv` -bestand bijvoorbeeld `crm_small.csv` is, moet het `.zip` -bestand `crm_small.csv.zip` zijn. Het bestand `.fin` moet overeenkomen met het bestand `.csv` . |


## Vereisten voor de kenmerkgegevensbestanden {#section_169FBF5B7BBA47CE825B7A330CF3FE98}

**Voorbeeld CSV**

Het CSV-bestand moet de volgende indeling hebben:

![ Vereisten voor de dossiers van attributengegevens ](assets/cvs.png)

Hetzelfde bestand wordt weergegeven in een teksteditor:

![ Vereisten voor de dossiers van attributengegevens ](assets/csv_txt.png)

**Richtlijnen**

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
   <td colname="col2"> <p>Het bestand voor slepen en neerzetten moet kleiner zijn dan 100 MB. </p> <p>Het bestand <span class="filepath"> .fin </span> is niet vereist wanneer u de uploadmethode voor slepen en neerzetten gebruikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>klant-id, kolom </p> </td> 
   <td colname="col2"> <p> De eerste kolom moet een unieke klant-id zijn. De gebruikte id moet overeenkomen met de id die wordt doorgegeven aan de Experience Cloud-id-service. </p> <p>Voor Analytics wordt de id opgeslagen in een prop of eVar. </p> <p>Voor Doel, de setcustomerID waarde. </p> <p> Deze klant-id is de unieke id die uw CRM gebruikt voor elke persoon in uw database. De resterende kolommen zijn attributen die uit uw CRM komen. U kiest hoeveel kenmerken u wilt uploaden. </p> <p>U kunt goed leesbare namen aanbevelen voor de kolomkoppen, maar deze zijn niet vereist. Wanneer u het schema na het uploaden valideert, kunt u vriendelijke namen toewijzen aan de geüploade rijen en kolommen. </p> <p> <b> Ongeveer klant IDs </b> </p> <p>Een onderneming gebruikt doorgaans een klant-id van een CRM-systeem. Deze id wordt ingesteld met de aanroep <span class="codeph"> setcustomerIDs </span> wanneer een persoon zich aanmeldt. Deze id wordt ook gebruikt als de sleutel in het CRM-bestand dat naar Experience Cloud wordt geüpload. Een <a href="t-crs-usecase.md" format="dita" scope="local"> alias-id </a> is een vriendelijke naam voor een gegevensopslag in Audience Manager, waar de aliasgegevens worden opgeslagen. Het systeem verzendt aliassen naar deze gegevensopslag (via setcustomerIDs). Het CRM-bestand wordt toegepast op de gegevens in die gegevensopslag. </p> <p>Zie <span class="codeph"> Customer ID's en verificatiestatussen </span> voor informatie over <a href="https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=nl-NL" format="https" scope="external"> setcustomerID's </a> . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Volgende koppen en kolommen </p> </td> 
   <td colname="col2"> <p>De volgende kopballen zouden de naam van elk attribuut moeten vertegenwoordigen. </p> <p> Deze kolommen zouden klantenattributen moeten bevatten die uit CRM komen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>kenmerklimieten </p> </td> 
   <td colname="col2"> <p>U kunt honderden kolommen <span class="filepath"> .csv </span> uploaden naar de klantenkenmerkservice in Experience Cloud. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten, afhankelijk van de toepassingen die u hebt: </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b> Norm van Analytics </b>: 3 totaal </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b> Premie van Analytics </b>: 200 per rapportreeks </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b> Adobe Target Norm:</b> 5 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b> Premium van Adobe Target:</b> 200 </li> 
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
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> Plaats het <span class="filepath"> .csv </span> -bestand (en het <span class="filepath"> .fin </span> -bestand) in de hoofdmap van de FTP-site. </li> 
     </ul> </p> <p> <p>Belangrijk: de totale hoeveelheid ruimte die voor de FTP-account is toegestaan, is 40 GB. Het is uw verantwoordelijkheid om verwerkte bestanden te verwijderen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bestandsvereisten </p> </td> 
   <td colname="col2"> <p> Elke kenmerkbron moet hetzelfde aantal door komma's gescheiden velden bevatten. </p> <p> Velden met een regeleinde, een dubbel aanhalingsteken of komma moeten worden opgegeven. </p> <p> Dubbele aanhalingstekens in een veld moeten worden voorkomen met een backslash (\). </p> <p> Lege kolommen worden opgeslagen als <span class="term"> null </span> . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Meerdere bestanden </p> </td> 
   <td colname="col2"> <p>Als u kenmerkgegevens van klanten uploadt en u meerdere bestanden hebt die u snel na elkaar wilt uploaden, en vooral als de bestanden groot zijn, moet u controleren of het vorige bestand is verwerkt voordat u het volgende bestand uploadt. U kunt dit controleren door te controleren wanneer het vorige bestand naar de verwerkte of mislukte map in uw [!DNL Customer Attributes] FTP-account is verplaatst. </p> <p> Wanneer u een groot bestand in kleinere bestanden splitst en snel na elkaar verzendt, kan dit de verwerking vertragen, tenzij u ervoor kunt zorgen dat elk bestand wordt verwerkt voordat het volgende bestand wordt verzonden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tekencodering </p> </td> 
   <td colname="col2"> <p>Voor Japan is UTF-8 verplicht. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>Historische gegevens </p> </td> 
   <td colname="col2"> <p> klantkenmerken zijn gekoppeld aan het onderliggende bezoekersprofiel in [!DNL Analytics] . [!DNL Customer Attributes] wordt daarom gedurende de gehele levensduur van dat bezoekersprofiel gekoppeld aan de bezoeker in [!DNL Analytics] . Dit profiel bevat gedrag dat is opgetreden voordat de klant zich voor het eerst heeft aangemeld. </p> <p> Als u de Data Warehouse backfill methode gebruikt, zijn de gegevens gekoppeld aan een post_visid_high/low die is gebaseerd op de Analytics ID (AID). Als u de Experience Cloud ID Service gebruikt, zijn de gegevens gekoppeld aan een post_visid_high/low die is gebaseerd op Experience Cloud ID (MID). </p> <p> De Data Warehouse backfill-methode is vanaf oktober 2022 niet meer beschikbaar. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gegevensfeeds </p> </td> 
   <td colname="col2"> <p>klantkenmerken zijn niet beschikbaar in gegevensfeeds. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Meerdere gegevensbronnen gebruiken {#multiple}

Wanneer het creëren van, het wijzigen van, of het schrappen van de bronnen van de klantenattributen, is er een vertraging rond één uur alvorens IDs met de nieuwe gegevensbron begint te synchroniseren.

Alias ID voor elke bron van klantkenmerken moet uniek zijn. Als u meerdere gegevensbronnen hebt die dezelfde id gebruiken, kunnen deze als volgt worden ingesteld:

**in VisitorAPI.js of het hulpmiddel van identiteitskaart van Experience Cloud in dynamisch markeringsbeheer:**

Stel twee klant-id&#39;s in die overeenkomen met de juiste gegevensbronnen:

```
Visitor.setcustomerIDs({ 
     "ds_id1":"123456", 
     "ds_id2":"123456" 
});
```

(Zie [ klant IDs en de Staten van de Authentificatie ](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=nl-NL) voor meer informatie.)

In **[!DNL Experience Cloud]** > **[!DNL Customer Attributes]** :

Maak twee bronnen voor klantkenmerken met behulp van unieke alias-id&#39;s die overeenkomen met de bovenstaande id&#39;s van de klant. Met deze methode kan dezelfde referentie-id naar meerdere bronnen voor klantkenmerken worden verzonden.
