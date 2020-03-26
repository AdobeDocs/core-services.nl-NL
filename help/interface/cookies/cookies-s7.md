---
description: Scene7 gebruikt koekjes om nuttige informatie op te slaan die aan levering dynamische media aan browser kan worden gebruikt.
keywords: cookies;privacy
seo-description: Scene7 gebruikt koekjes om nuttige informatie op te slaan die aan levering dynamische media aan browser kan worden gebruikt.
seo-title: Scene7 Cookies
solution: Marketing Cloud,Analytics,Target,Social
title: Scene7 Cookies
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
translation-type: tm+mt
source-git-commit: 012283d79bda42f9dabb20b25903927b075f6d54

---


# Scene7 Cookies{#scene-cookies}

Scene7 gebruikt koekjes om nuttige informatie op te slaan die aan levering dynamische media aan browser kan worden gebruikt.

Scene7 slaat plaatselijk informatie voor sommige oudere AS2 op flits gebaseerde kijkers op.

Voor AS2-viewers, cookies:

* De sessiestatus van een gebruiker bijhouden, zoals de huidige pagina en de weergegeven afbeelding, het huidige zoomniveau enzovoort.
* Bepaal hoe lang het sinds de vorige zitting van de gebruiker is geweest. De viewer gebruikt deze informatie om te beslissen of een vorige sessie moet worden voortgezet of dat een nieuwe sessie moet worden gestart. Deze informatie wordt ook verzonden naar de servers Scene7, maar dat wordt niet gebruikt.

Voor AS2 Flash eCatalog-viewer, cookies:

* Door de gebruiker gegenereerde inhoud opslaan (met name inhoud die door de gebruiker is ingevoerd in de functie &quot;sticky notes&quot; van de catalogusviewer). Deze inhoud wordt hersteld wanneer de gebruiker een sessie hervat.
* Wanneer de gebruiker een e-mail initieert om de catalogus met een andere gebruiker te delen, wordt de inhoud van de sticky notes van het tweede AS2-vieweropsommingsteken naar onze servers gekopieerd om het aan de ontvanger te verstrekken. Wanneer de ontvanger de viewersessie start, wordt de inhoud van de plaknotities opgehaald van de server en gekopieerd naar een cookie. Deze functie wordt weinig gebruikt, dus de functie verloopt niet en de inhoud van de schaal wordt niet verwijderd. Op dit ogenblik blijft het op de servers voor onbepaalde tijd voortbestaan.

De nieuwere AS3-viewers implementeren sessieresistentie niet.

**Naam cookie: VatLogin.jsp**

| Kenmerk | Beschrijving |
|---|---|
| Opgeslagen informatie | Stelt het sessiecookie in. AuthFilter ingebed in IPS ImageServer (IS, IR, en ook SWFs/skins en videocontexten) gebruikt het koekje voor toegangsvergunning. Indien aanwezig, staat het HTTP- verzoeken toe om door te gaan. Anders wordt onbevoegd geretourneerd. |
| Verlopen | Dit cookie is een sessiecookie. De huidige zittingsafloop wordt geplaatst aan 45 minuten in Scene7 IPS [!DNL web.xml]. |

**Naam cookie: s7js.flyout.InfoMessage.displayed`assetId`.state**

<table id="table_6835D64C5D464A049F576621F2BE3FAD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Opgeslagen informatie </td> 
   <td colname="col2"> <p>&lt;assetId&gt; is de naam van het element waarmee de viewer werkt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Verlopen </td> 
   <td colname="col2"> Dit cookie is een sessiecookie en verloopt wanneer de browser wordt gesloten. </td> 
  </tr> 
 </tbody> 
</table>

**Naam cookie: s7js.flyout.InfoMessage.displayed`assetId`_idx`id`.ant**

Browsercookies worden door verouderde DHTML-viewers gebruikt voor het opslaan van statusinformatie en sticky notes-gegevens. Ze worden ook gebruikt door de DHTML-flyout voor meerdere schermen voor het specifiek maken van berichtindicatorsessies.

<table id="table_8F6CC83D32D54BEE99884318AD126C98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Kenmerk </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Opgeslagen informatie </td> 
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; is de naam van het element waarmee de viewer werkt en &lt;id&gt; is de op nul gebaseerde index voor notities. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Verlopen </td> 
   <td colname="col2"> Dit cookie is een sessiecookie en verloopt wanneer de browser wordt gesloten. </td> 
  </tr> 
 </tbody> 
</table>
