---
description: Functies, opmerkingen bij releases en bekende problemen voor de Experience Cloud-interface.
keywords: core services
seo-description: Functies, opmerkingen bij releases en bekende problemen voor de Experience Cloud-interface.
seo-title: Opmerkingen bij de cumulatieve release
solution: Experience Cloud
title: Opmerkingen bij de cumulatieve release
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
translation-type: tm+mt
source-git-commit: 31811e718be130612c8688e80084cb7579e94f47

---


# Opmerkingen bij de cumulatieve release

Functies, opmerkingen bij releases en bekende problemen voor de Experience Cloud-interface.

Zie [Experience Cloud](../doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784)voor een lijst met documentatie-updates.

Zie Opmerkingen bij de release [Experience Cloud voor opmerkingen bij](https://docs.adobe.com/content/help/en/release-notes/experience-cloud/current.html)de release.

## Januari - 2020

* De pagina Feed is in december 2019 afgekeurd. Zoek naar een bericht over afgekeurde producten. (MCUI-10039)

## Augustus - 2019

* Oplossing voor een kritiek probleem in de aanmeldingsgegevens voor Experience Cloud dat tot een sessieafmelding voor sommige gebruikers heeft geleid. (MCUI-6908)
* Aanmelden bij Experience Cloud om de prestaties te verbeteren en de latentie te verminderen. (MCUI-6854, MCUI-6869, MCUI-6883)
* Bijgewerkte interface cosmetisch. (MCUI-6861, MCUI-6911, MCUI-6862)
* Probleem verholpen met Experience Cloud [!UICONTROL Triggers] die leidde tot een onjuiste interpretatie van de _like_ clausule in de definitie van [!UICONTROL Trigger] . (MCUI-6611)

## April - 2019

* De app-switch is bijgewerkt en bevat Marketo in Experience Cloud-oplossingssuite en brandingsupdates voor Experience Platform. (MCUI-6529)
* Bijgewerkte Experience Cloud Home om navigatiekoppelingen naar de pagina&#39;s Feed en Administration op te nemen. (MCUI-6682)
* Probleem verholpen in de definitie [!UICONTROL Trigger] voor correct gebruik van de clausule &#39;like&#39;. (MCUI-6611)
* Verbeteringen aan de Attributen van de Klant voor beter het registreren in de dienst van het Abonnement. (MCUI-6519)

## Release 19.1.1 - 17 januari 2019

**Opmerking:** In maart 2019 biedt de Experience Cloud-interface geen ondersteuning voor Internet Explorer 11.

* Probleem verholpen waarbij het zoeken naar Help niet tot resultaten leidde. (MCUI-1670)
* Vast en verbeterd eVar-beheer in Triggers. (MCUI-6400)

## Release 16.5.1 - 26 mei 2016 {#section_3785F182BC13493F84903CA69EB6D0A8}

**Functies en verbeteringen**

<table id="table_ABBCE1A66F534059BD728BC2B9AEFA80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Vooraf geconfigureerde productconfiguraties in de beheerconsole </p> </td> 
   <td colname="col2"> <p>Cloud-klantbeheerders kunnen productconfiguraties gebruiken die vooraf zijn gemaakt en zijn toegewezen aan standaardmachtigingsgroepen voor Analytics en Dynamic Tag Management. </p> <p>Deze optimalisatie is beschikbaar voor nieuwe organisaties en beperkt de tijd die organisaties nodig hebben om gebruikers in de beheerconsole te beheren. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Voederverbetering </p> </td> 
   <td colname="col2"> <p> Als u een nieuwe post maakt in de Cloudinvoer voor ervaring, gebruikt de regel Aan nu het actieve onderwerp in plaats van de organisatie standaard.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij miniaturen niet konden zien voor elementen die werden gedeeld van Assets op aanvraag naar de Experience Cloud Feed. (MAC-29955)

## Release 16.2 februari 2016 {#section_D9610373116C4D77A38F67815C725EA3}

<table id="table_C9B288CF42034F329C3C72D95D22E515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Verbeteringen in de cloud-elementen </p> </td> 
   <td colname="col2"> <p>In Experience Cloud Assets kunt u uw digitale middelen opslaan, delen en synchroniseren vanaf één centrale locatie. Experience Cloud Assets gebruikt een aantal van de functies die beschikbaar zijn in <span class="keyword"> Adobe Experience Manager</span> (AEM). </p> <p>Zie <a href="../experience-cloud-assets/experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local"> Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verbeteringen voor het koppelen van accounts </p> </td> 
   <td colname="col2"> <p>Verbeterde interfaceworkflow voor het koppelen van oplossingsaccounts aan de Experience Cloud (Adobe-id). Deze nieuwe workflow zoekt alle accounts van de gebruiker die aan een organisatie zijn gekoppeld en geeft u de mogelijkheid om te kiezen welk account aan een koppeling wordt gekoppeld. We hebben ook de koppelingservaring voor accounts gestroomlijnd, zodat u de pagina Organisaties beheren niet meer hoeft te openen om accounts handmatig te koppelen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij koppelingen en SSO voor Analytics werden voorkomen. Deze kwestie toonde de &quot;Bericht: Het foutbericht: FOUT IMS SSO is mislukt: Kan het gekoppelde bedrijf niet vinden.&quot;

**Bekend probleem**

Als u via de interface **[!UICONTROL Experience Cloud]** > **[!UICONTROL Activation]** toegang krijgt tot Dynamic Tag Management, maar uw Dynamic Tag Management-account is niet gekoppeld aan de Experience Cloud (Adobe-id), kunt u zich niet aanmelden bij Dynamic Tag Management. Navigeer rechtstreeks naar een nieuw browsertabblad om dit probleem te voorkomen. [!DNL dtm.adobe.com]

## Release 16.1 - januari 2016 {#section_33B3F7DF6CA347E3AA93801BAC6232CE}

<table id="table_4223658257DA41C999AC710A10D26771"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Poortbibliotheek-berichten </td> 
   <td colname="col2"> <p> Wij verbeterden de Bibliotheek van het Publiek om nuttige berichten te omvatten wanneer het bouwen van publiek of wanneer een onderbreking voorkomt. </p> <p>Wanneer u bijvoorbeeld meer dan vijf regels toevoegt, wordt een bericht weergegeven dat aangeeft dat u de maximaal toegestane regels hebt overschreden. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Microsoft [beëindigt steun](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) voor Internet Explorer 8, 9, en 10. Als zodanig, zullen wij geen kwesties bevestigen die tegen deze specifieke versies van Internet Explorer worden gemeld.

## Release 15.10 - 14 oktober 2015 {#section_68123833D3634BD3A473C12862BF9606}

**Bekende problemen**

* Klanten kunnen zich niet aanmelden bij Report Builder als ze via de Experience Cloud toegang hebben tot Analytics. Dit probleem is niet van invloed op klanten die oude analysegegevens gebruiken.
* Bekende kwestie met de &quot;Verbinding aan de functie van het Rapport&quot;in Analytics. Klanten die zich via de Experience Cloud aanmelden bij Analytics, worden naar een niet-SSO-aanmeldingspagina gestuurd wanneer ze een rapport proberen te delen.

## Release 15.9 - 10 september 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Oplossing voor een probleem met de API-prestaties van Audience Manager dat tot periodiek onderbrekingen leidde bij het uploaden van klantkenmerkgegevens. (MAC-26305)
* Probleem verholpen waarbij gebruikers maximaal 200 klantkenmerken aan een abonnement konden toevoegen. (MAC-26188)
* Probleem verholpen met Audience Library die ervoor zorgde dat het delen van het publiek niet werd beïnvloed door segmentering van Analytics. Dit probleem heeft ertoe geleid dat &quot;Gegevens verzamelen&quot; (0 soorten publiek) werd weergegeven. Om dit probleem te voorkomen, raadt Adobe aan de segmentgrootte onder de 50 kB te houden. (MAC-25788)
* Oplossing voor een eerder bekend probleem met de kenmerken van de klant - Bewerk de pagina Schema die een fout met behoud van inhoud veroorzaakte die werd gegenereerd bij het wijzigen van een weergavenaam. (MAC-25589, AN-103834)

## Release 15.7 - juli 2015 {#section_2683A152176944E48EF6C943892975B7}

* Probleem verholpen waardoor kenmerkbeschrijvingen die zijn opgegeven op de pagina Weergeven/Schema bewerken (in klantkenmerken) niet konden worden bijgewerkt in analyserapporten. (MAC-25985)
* Probleem verholpen waarbij de miniaturen niet konden worden gerenderd voor geüploade elementen. (MAC-25863)
* Probleem verholpen waardoor nieuwe segmenten die in rapporten en analyses zijn gemaakt, niet beschikbaar waren in Experience Cloud Audiences. (MAC-25817)
* Probleem verholpen waarbij delen van publiek door Analytics werd voorkomen bij gebruik van de service bezoekersidentiteitskaart. (MAC-25788, MAC-25747)
* Extra ondersteuning voor multibyte-tekens in klantkenmerken. (MAC-2552)

**Bekend probleem**

Een bekend probleem leidt ertoe dat dubbele automatisch gegenereerde accounts worden gemaakt in Audience Manager en dat deze automatisch worden gekoppeld aan de Cloud-identiteit van een gebruiker. Dit probleem doet zich voor als u naar Audience Manager navigeert voordat u uw accounts koppelt. Adobe raadt u aan uw accounts in Audience Manager te koppelen aan de Experience Cloud voordat u naar Audience Manager navigeert. (MAC-25640)

## Release 15.6.1 - 11 juni 2015 {#section_AD2019F8D2F84C9EB2B0533FAACF7043}

Geen informatie beschikbaar

## Release 15.5.1 - 13 mei 2015 {#section_EF197410964E40D294D0D8024738CFBA}

<table id="table_14E7B35E06C84A258A21D09691B58354"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>De linkernavigatiemenu's zijn bijgewerkt en gerangschikt om toegang tot alle kerndiensten en oplossingen te verlenen. Opmerkelijke wijzigingen zijn: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">De selecties in het menu <span class="term"> Audience Library</span> en <span class="term"> Customer Attributes</span> bevinden zich nu onder <span class="term"> Publiek</span>. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">De selectie van het menu <span class="term"> Exchange</span> -menu is verplaatst van het vervolgkeuzemenu Help naar de linkernavigatiespoor. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> <span class="term"> Oplossingen</span> zijn verwijderd. U kunt alle oplossingen lanceren vanaf de onderste helft van de navigatieregel. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Probleem verholpen waarbij werd voorkomen dat klantkenmerken voor sommige klanten werden gesynchroniseerd.
* Oplossing voor een probleem dat ervoor zorgde dat de pagina met [Adobe Target-productdocumentatie](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html) niet kon worden weergegeven in het Japans.
* Probleem verholpen waarbij het gebruik van Japanse tekst in opmerkingen tussen de [!DNL Creative Cloud] en de [!DNL Experience Cloud].

## Release 15.4.1 - 8 april 2015 {#section_75634120CC934B3381EDEA7F6F976F0A}

<table id="table_3A6FBAE36558425A803B078150862C92"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Verbeteringen voor beheer: </p> 
    <ul id="ul_7D5FCBEFA262435D865CA1018BFB792E"> 
     <li id="li_6E98974CCB094ABBAB57C51ED56C3F00"> <span class="wintitle"> Admin Console</span> </li> 
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Ondersteuning voor Enterprise en federatieve id </li> 
    </ul> </td> 
   <td colname="col2"> <p>De functionaliteit voor gebruikers- en groepsbeheer is verplaatst naar de beheerconsole. Het nieuwe navigatiepad is: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Beheer</span> &gt; Admin Console <span class="uicontrol"> starten</span></p> <p> Er is ook ondersteuning toegevoegd voor bedrijfs- en gefedereerde id's. U kunt bedrijfs-id's, gefedereerde id's en Adobe-id's gebruiken in dezelfde implementatie voor ondernemingen. Gebruik bijvoorbeeld Adobe-id's voor gebruikers die andere Adobe-producten en -services kunnen gebruiken. Gebruik bedrijf- of gefedereerde id's voor gebruikers waar u hun accounts strikt wilt beheren. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij Single Sign-On tussen [!DNL Experience Cloud] en [!DNL Media Optimizer].

**Bekende problemen**

* Het koppelen en ontkoppelen van uw dynamische organisatie voor tagbeheer aan de Experience Cloud werkt niet voor nieuwe Experience Cloud-organisaties. We zijn bezig dit probleem op te lossen en de normale functionaliteit te herstellen met de release van mei. Als u problemen ondervindt bij het aanmelden bij dynamisch tagbeheer via de Experience Cloud, kunt u zich aanmelden bij [!DNL dtm.adobe.com]de oudere versie.
* Een bekend probleem is dat het delen van het publiek wordt verhinderd door het rapporteren van suites die niet het eigendom zijn van de gekoppelde account Analytics. Er wordt gewerkt aan corrigerende maatregelen

## Release 15.3.2 - 19 maart 2015 {#section_07760FD9CA43497FA8BDCCA990A24BFD}

<table id="table_54025DBE2D094FF1BE837BA60816C6DF"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Klantkenmerken </p> </td> 
   <td colname="col2"> <p>Als u gegevens van ondernemingsklanten in een gegevensbestand van het het relatiebeheer van de klant (CRM) vangt, kunt u de gegevens in een gegevensbron van de klantenattributen in de Wolk van de Ervaring uploaden. Nadat de gegevens zijn geüpload, kunt u de rapporten <span class="uicontrol"> Bezoekersprofiel</span> &gt; Klantkenmerken <span class="uicontrol"></span> uitvoeren in Analytics. </p> <p>U kunt de geüploade gegevens ook gebruiken als een publiekssegment in <span class="keyword"> Adobe Target</span>. </p> <p>Raadpleeg de <a href="../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1" format="dita" scope="local"> productdocumentatie van Kenmerken</a> van de klant. </p> <p> Voor informatie over het moderniseren van uw oplossingen voor de kerndiensten, zie <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Uw oplossingen voor de kerndiensten</a>toelaten. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Release 15.3.1 - 4 maart 2015 {#section_57CB69C044DD47BDBC1A1BEC38957551}

<table id="table_EB3FFBA2DF904546A5185EC9A63BBA98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Groepstoewijzing </p> </td> 
   <td colname="col2"> <p>De pagina Groepsbeheer is opnieuw ontworpen als een beheerinterface waarmee u groepen kunt maken, gebruikers aan groepen kunt toevoegen en machtigingen kunt toepassen voor de verschillende oplossingen van de Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Toewijzing van één naar veel </p> </td> 
   <td colname="col2"> <p>Als u oplossingsaccounts koppelt in de Experience Cloud en meerdere oplossingen en organisaties hebt, kunt u nu meerdere producten en services toewijzen aan één organisatie. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activering </p> </td> 
   <td colname="col2"> <p> <a href="../activation/activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local"> Activering</a> wordt nu weergegeven in de navigatie links in de <span class="keyword"> Experience Cloud</span>. <span class="wintitle"> Activering</span> is een <span class="keyword"> Experience Cloud</span> -service die momenteel bestaat uit de technologie voor dynamisch tagbeheer en die u de instructie geeft wanneer erop wordt geklikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Documentatie-updates - Core Services </p> </td> 
   <td colname="col2"> <p>Toegevoegd het onderwerp <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> laat uw oplossingen voor de kerndiensten</a> toe om u bij het uitvoeren van de kerndiensten te helpen. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Release 15.2.1 - 19 februari 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Oplossingen:

* Verbeterde werkstroom voor e-mailuitnodigingen van gebruikers voor het instellen van accounts.
* Probleem verholpen met een elementmap waardoor identieke maphiërarchieën niet konden worden weergegeven [!DNL Experience Cloud] [!DNL Adobe Campaign] en elementen niet konden worden weergegeven.
* Oplossing van een probleem dat de verwijdering van publiek dat deel uitmaakte van gedeactiveerde [!DNL Target] activiteiten, verhinderde.
* Probleem verholpen waarbij het pictogram Toevoegen (plus) niet kon worden weergegeven onder [!UICONTROL Regels] op de pagina [!UICONTROL Nieuw publiek] maken.
* Verbeterde ondersteuning voor de Cloud-interface voor Internet Explorer 9.

## Release 15.1.1 - 15 januari 2015 {#section_F1A352E928AF432E94CC0A289C345184}

Nieuwe functies en oplossingen in de interface voor [!DNL Adobe Experience Cloud] samenwerken en delen.

<table id="table_AD0A8CA760E64227BB04BA6B0E425E80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Alleen-lezen toegang. </p> </td> 
   <td colname="col2"> <p>Beheerders kunnen niet-administratieve gebruikers nu alleen-lezen toegang verlenen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Correctie van een probleem waarbij PNG-bestanden niet konden worden gerenderd op een kaart.
* Probleem verholpen met het uploaden van bestanden naar Experience Cloud Assets via slepen en neerzetten.

**Bekende problemen**

* Gebruikers kunnen PowerPoint-bestanden niet delen op borden.
* Wijzigingen in groepen en machtigingen die zijn aangebracht in Gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen problemen ondervinden bij het uploaden van grote bestandstypen naar Experience Cloud Assets.
* Gebruikers ontbreken mogelijk koppelingen op hun Experience Cloud-kaarten van Media Optimizer.
* Sommige administratieve gebruikers kunnen problemen ervaren met hun accounts nadat ze een uitnodiging hebben geaccepteerd om deel te nemen aan de Experience Cloud.
* De Experience Cloud-interface kan de prestaties verlagen wanneer deze gelijktijdig door meerdere gebruikers worden gebruikt.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Sommige gebruikers kunnen problemen ondervinden wanneer ze zich gelijktijdig aanmelden bij twee browsers met dezelfde Adobe-id.
* Sommige gebruikers kunnen een Creative Cloud-gebruiker niet opnieuw toevoegen aan een gedeelde map nadat de Creative Cloud-gebruiker is verwijderd.
* Sommige gebruikers ondervinden mogelijk een vertraging in de melding die optreedt wanneer een map wordt gedeeld vanuit de Experience Cloud naar Creative Cloud.
* Sommige gebruikers ondervinden mogelijk problemen bij het delen van een map tussen de Experience Cloud en Creative Cloud.
* Sommige gebruikers kunnen problemen ondervinden bij het maken van een publiek in een Analytics-rapportensuite nadat het gedeelde publiek is ingeschakeld.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.

## Release 14.11.1 - 13 november 2014 {#section_A6CF1D4F27B9496892A89C983EB39102}

Bekende problemen:

* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden weergegeven.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Beheerders moeten zich afmelden en weer aanmelden om de wijzigingen te kunnen zien die in Accountinstellingen zijn aangebracht.
* De gebruiker kan geen PowerPoint-bestanden op borden delen.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* Adobe Experience Manager voor synchronisatie met Creative Cloud werkt niet.

## Release 14.10.1 - 16 oktober 2014 {#section_E3A0F4423B814707AA3745E083500835}

Nieuwe functies en oplossingen in de interface voor [!DNL Adobe Experience Cloud] samenwerken en delen.

<table id="table_7C1ACE8108D54782AE128ACD35069DF5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gebruikersmachtigingen bewerken </p> </td> 
   <td colname="col2"> <p>Eigenaars van een board kunnen nu gebruikersmachtigingen op de betreffende board bewerken. </p> <p> 
     <ol id="ol_B12251C510744538AF9BCE60ACB04016"> 
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">Klik op <span class="uicontrol"> Instellingen</span>in het bord. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Geef naast elke eigenaar de <span class="uicontrol"> eigenaar</span>, de <span class="uicontrol"> Viewer</span>of de <span class="uicontrol"> Editor</span>op. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Er werd een foutbericht geretourneerd wanneer u een kaart maakte van een PDF en deze naar het bord deelde.

**Bekende problemen**

* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden weergegeven.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* De gebruiker kan geen PowerPoint-bestanden op borden delen.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .

## Release 14.9.1 - 18 september 2014 {#section_20F156A9CC2F4FC59C4970075C181D3A}

**Oplossingen en verbeteringen**

* Wanneer u naar [!DNL experiencecloud.adobe.com]deze locatie navigeert, is de aanmeldingservaring nu consistent met de Creative Cloud-aanmelding van Adobe.
* Op de pagina Organisaties beheren is de koppelingservaring (nadat een uitnodiging is ontvangen) nu consistent voor elke oplossing.

**Bekende problemen**

* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* De gebruiker kan geen PowerPoint-bestanden op borden delen.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden weergegeven.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud] inhoud uit hun omslag wordt verwijderd, als de inhoud niet gedeeld in [!DNL Experience Cloud].

## Release 14.8.1 - augustus 2014 {#section_03BF00F6A95A490C91BCC0A1988FA7AA}

Nieuwe functies en oplossingen in de interface voor [!DNL Adobe Experience Cloud] samenwerken en delen.

<table id="table_1E7DBEB5E83B4E4285B6FD1D718CD16D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>U hebt nu toegang tot <span class="keyword"> Adobe Mobile Services</span> vanuit de linkernavigatie. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekende problemen**

* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige gebruikers kunnen zich mogelijk niet aanmelden van [!DNL Target] naar [!DNL Experience Cloud].
* Sommige gebruikers van Audience Manager kunnen zich niet aanmelden bij de [!DNL Experience Cloud].
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* De gebruiker kan geen PowerPoint-bestanden op borden delen.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden weergegeven.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud] inhoud uit hun omslag wordt verwijderd, als de inhoud in unshared in [!DNL Experience Cloud]. is.

## Release 14.7.1 - juli 2014 {#section_B22D4F830756463DB27BB4D508D9ADD5}

Nieuwe functies en oplossingen in de interface voor [!DNL Adobe Experience Cloud] samenwerken en delen.

**Bekende problemen**

* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* Sommige [!UICONTROL gebruikers van de Uitwisseling] kunnen hun namen in de commentaren vinden om een lange koordidentiteitskaart in plaats van hun namen te zijn
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden gerenderd
* Bij het uploaden van bestanden zijn meer bestandstypen toegestaan dan bij slepen en neerzetten. Upload het bestand met [!UICONTROL Elementen]voor de beste resultaten.
* De [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .
* [!DNL Exchange] gebruikers moeten hun cookies wissen om hun ervaring te verbeteren.
* [!DNL Experience Cloud] de interface kan vertragen wanneer in parallel gebruik door vele gebruikers.
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud] inhoud uit hun map wordt verwijderd als de inhoud niet wordt gedeeld in de [!DNL Experience Cloud]map.
* U wordt afgemeld na 15 minuten inactiviteit. Bovendien wordt u door het afmelden op één locatie afgemeld bij het [!DNL Experience Cloud]programma.
* Sommige gebruikers kunnen hun accounts in Audience Manager niet koppelen aan [!DNL Experience Cloud].
* [!UICONTROL De gebruikers van de uitwisseling] kunnen Engels in taalselecteur slechts zien.

**Oplossingen**

Geen om te rapporteren.

## Release 14.6.1 - 19 juni 2014 {#marketing_cloud_interface}

Nieuwe functies en oplossingen in de interface voor [!DNL Adobe Experience Cloud] samenwerken en delen.

**Verbetering**

<table id="table_C9BD63436BF0414B97B8D07387D1993B"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="wintitle"> Knop Opslaan</span> in Soorten publiek </p> </td> 
   <td colname="col2"> <p>Wanneer u een publiek maakt, wordt de knop <span class="wintitle"> Opslaan</span> op de pagina Nieuw publiek <span class="wintitle"></span> maken nu uitgeschakeld totdat alle vereiste velden zijn voltooid. 
     <!--MAC-19712 --></p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekende problemen**

* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* Bij het uploaden van bestanden zijn meer bestandstypen toegestaan dan bij slepen en neerzetten. Upload het bestand met Middelen voor de beste resultaten.
* De [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in de [!DNL Experience Cloud]map.
* Sommige gebruikers kunnen hun account voor publieksbeheer niet koppelen aan hun [!DNL Experience Cloud] account.
* U wordt afgemeld na 15 minuten inactiviteit. Als u zich afmeldt op één locatie, meldt u zich bovendien af van de Experience Cloud.
* Sommige gebruikers van de Uitwisseling kunnen hun namen in de commentaren vinden om een lange koordidentiteitskaart in plaats van hun namen te zijn

**Oplossingen**

* Probleem verholpen waarbij het uploaden van video&#39;s naar apps werd voorkomen.

## Release 14.5.1 - mei 2014 {#section_7E22B2CB3ABA4D6EAED8CA8EFDE5433E}

<table id="table_4E4B34EEE3D94D78BA1A1FBC62950559"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Exchange </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Help</span> &gt; <span class="uicontrol"> Exchange</span></p> <p>De <span class="keyword"> Experience Cloud</span><span class="wintitle"> Exchange</span> is één bestemming waar u digitale marketingextensies kunt zoeken, zoeken, selecteren, betalen en downloaden via apps. </p> <p>Tot de toepassingen behoren gegevensconnectors, aangepaste configuraties voor het kernproduct van Adobe, toepassingen van derden, rapporten en <span class="keyword"> Experience Cloud</span> -kaarten. </p> <p>Zie <a href="../exchange.md#concept_E07F16F070544B82B56527A845C41D59" format="dita" scope="local"> Exchange Marketplace</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cloud-publiek beleven </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Soorten publiek</span></p> <p> <span class="wintitle"> Het publiek</span> is waar u creeert, uitgeeft, en leidt publiek, gelijkend op hoe u met segmenten werkt. U kunt bijvoorbeeld een segment maken in rapporten en analyses en dit delen naar <span class="wintitle"> Experience Cloud</span><span class="wintitle"> Audiences</span>. Als de doelgroep eenmaal is gedeeld, is deze beschikbaar in <span class="keyword"> Adobe Target</span> voor campagneactiviteiten en in Adobe Audience Manager voor segmentering. </p> <p> <p>Opmerking: Ga naar <a href="https://www.adobe.com/go/audiences" format="http" scope="external"> https://www.adobe.com/go/audiences</a>om activering in Target aan te vragen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Gebruikers die op de <span class="keyword"> Experience Cloud</span> -kaarten worden vermeld, hebben nu machtigingen voor die kaart. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>De nieuwe gebruikers van Adobe kunnen hun rekeningen Scene7 met identiteitskaart van Adobe evenals hun teamleden verbinden. De beheerders kunnen gebruikers van rekeningen ook losmaken Scene7. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Asset-synchronisatie. </p> </td> 
   <td colname="col2"> <p> U kunt middelen in Adobe Experience Manager (AEM)-middelen delen met Adobe Experience Cloud en Adobe Creative Cloud, zodat eventuele wijzigingen in deze middelen worden weerspiegeld in de gedeelde kopieën van de middelen in Adobe Experience Cloud en Adobe Creative Cloud. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* [!DNL Experience Cloud] was niet verbonden met [!DNL Adobe Target]. Dit probleem is opgetreden als de [!DNL Adobe Target] aanmelding op meerdere [!DNL Target] servers kan worden gebruikt.
* [!DNL Adobe Media Optimizer] heeft niet automatisch gebruikers gemaakt wanneer de gebruiker is aangemaakt in [!DNL Experience Cloud].
* Opties in keuzelijsten met invoervak die worden gebruikt voor het tijdelijk toevoegen van nieuwe gebruikers zijn tijdens het typen verdwenen.
* Er kan niet op de koppeling Opmerkingen in de weergave voor de kaart van het element worden geklikt.
* Nadat u een aangepaste tag aan een element hebt toegevoegd, zijn er geen andere metagegevenswijzigingen meer.
* Als u een afbeelding verwijdert, wordt er niet door Middelen gewaarschuwd of de afbeelding wordt gebruikt in Adobe Target Essentials.
* Trage [!UICONTROL Ervaring met de prestaties van de Cloud] -interface bij parallel gebruik door veel gebruikers.
* Als u een afbeelding verwijdert in [!UICONTROL Experience Cloud Assets] , verschijnt er geen waarschuwing als de afbeelding is gebruikt in [!DNL Adobe Target Essentials].
* Wanneer **** onthoud dat ik tijdens het aanmelden niet was geselecteerd, werd de gebruiker na 15 minuten afgemeld.
* Gebruikers moesten zich afmelden en weer inloggen om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Aanmelden bij de [!DNL Experience Cloud] server duurde langer dan een seconde.
* Voor bepaalde gebruikers synchroniseerde het schrappen van dossiers van de [!DNL Experience Cloud] niet met [!DNL Digital Asset Management].
* Gebruikers werden afgemeld na slechts 15 minuten browserinactiviteit.
* De gebruiker kon geen PowerPoint-bestanden op borden delen.
* Sommige gebruikers hadden in Internet Explorer 10 een slechte visuele lay-out dan andere browsers.

## Release 14.4.1 - 22 april 2014 {#section_E2A699764E744D2E8D418E9A3D40AF6B}

<table id="table_D95C0DC64F2A4B47BAC83E504CFD6825"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Kaarten maken van Help-onderwerpen </p> </td> 
   <td colname="col2"> <p>Nadat u de functie Delen naar Adobe Experience Cloud hebt ingeschakeld in de werkbalk Bladwijzer van uw browser, kunt u nu Help-pagina's delen via de URL van de microsite. </p> <p> <b>Een Help-onderwerp delen</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Klik in de <span class="keyword"> Experience Cloud</span>op <span class="uicontrol"> Beheer</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Sleep de knop <span class="uicontrol"> Delen naar Adobe Experience Cloud</span> naar de werkbalk Bladwijzer. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navigeer naar een Help-pagina (of blijf op deze pagina) en klik vervolgens op <span class="uicontrol"> Delen naar Adobe Experience Cloud</span> op de werkbalk Bladwijzers van uw browser. </p> <p>Met deze stap maakt u een kaart die u kunt weergeven in de <span class="wintitle"> Experience Cloud</span>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Nadat u een aangepaste tag aan een element hebt toegevoegd, kunnen er geen andere metagegevenswijzigingen meer worden doorgevoerd.
* Gebruikers moeten het bord vernieuwen om de verwijderde kaarten uit het zicht te laten verdwijnen.
* Wanneer **[!UICONTROL Onthoud dat ik]** niet is geselecteerd tijdens de aanmelding, wordt de gebruiker na 15 minuten afgemeld
* [!DNL Analytics] de openingspagina van de oplossing toont formatterende fouten.
* Gebruikers dienen zich af te melden en zich weer aan te melden om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Als u een afbeelding verwijdert, wordt er in [!UICONTROL Elementen] niet gewaarschuwd of de afbeelding wordt gebruikt in [!DNL Adobe Target Essentials].
* Er kan niet op de koppeling Opmerkingen in de weergave met de elementenkaart worden geklikt.
* Opties in keuzelijsten met invoervak voor het tijdelijk toevoegen van nieuwe gebruikers verdwijnen tijdens het typen.
* Aanmelden bij de [!DNL Experience Cloud] printer duurt langer dan een seconde.
* Gegevens die worden gedeeld vanuit [!DNL Media Optimizer] is onjuist weergegeven in de [!DNL Experience Cloud]map.
* Adobe maakt [!DNL Media Optimizer] niet automatisch gebruikers wanneer de gebruiker in de [!DNL Experience Cloud]toepassing is gemaakt.
* Er kan geen koppeling [!DNL Experience Cloud] worden gemaakt naar de map [!DNL Adobe Target]als de [!DNL Adobe Target] aanmelding op meerdere [!DNL Target] servers kan worden gebruikt.
* [!DNL Experience Cloud] de interface kan vertragen wanneer in parallel gebruik door vele gebruikers.
* [!DNL Search&Promote] koppeling is niet beschikbaar op de pagina [!UICONTROL Organisaties en producttoegang] .
* [!DNL Adobe Media Optimizer] simulatiekaarten worden niet correct weergegeven.
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in [!DNL Experience Cloud].
* Filters die worden toegepast op trended-rapporten van Analytics worden niet toegepast op kaarten in Experience Cloud.
* Sommige Excel- of CSV-bestanden kunnen niet naar een board worden geüpload.
* Sommige gebruikers kunnen hun account voor publieksbeheer niet koppelen aan hun [!DNL Experience Cloud]account.
* Sommige gebruikers kunnen een fout ervaren bij het delen van [!DNL Analytics] segmenten in de [!DNL Experience Cloud]app.
* Sommige gebruikers kunnen mogelijk niet naar submappen in [!UICONTROL Asset Selector]gaan.
* Sommige gebruikers kunnen geen AdLens-gadgets delen in de [!DNL Experience Cloud]app.

## Release 14.3.1 - 13 maart 2014 {#section_5D142E3225E3477A84DC01B8197D39BC}

Versie 14.3.1 is een onderhoudsrelease die zich richt op snelheid, stabiliteit en beveiliging. Belangrijke nieuwe functies worden niet opgenomen.

**Oplossingen**

* Hiermee kunt u uw avatar-afbeelding verwijderen.
* Probleem verholpen waarbij je je [!DNL Adobe Media Optimizer] accounts niet kon ontkoppelen.

**Bekende problemen**

* Als u een afbeelding verwijdert in Experience Cloud Assets, wordt niet gewaarschuwd of de afbeelding wordt gebruikt in Adobe Target Essentials.
* Het vernieuwen van een kaart van [!DNL Analytics] kan soms tot een leeg diagram in de uitgebreide kaart leiden.
* Gebruikers dienen zich af te melden en zich weer aan te melden om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Wanneer *`Remember me`* deze optie niet is geselecteerd tijdens het aanmelden, wordt de gebruiker na 15 minuten afgemeld.
* [!DNL Analytics] de openingspagina van de oplossing toont formatterende fouten.
* U kunt niet klikken op de koppeling Opmerkingen in de weergave met de elementenkaart.
* De interface van de Wolk van de ervaring kan vertragen wanneer in parallel gebruik door vele gebruikers
* Experience Cloud kan niet worden gekoppeld [!DNL Adobe Target], als de [!DNL Adobe Target] aanmelding kan worden gebruikt op meerdere doelservers.
* Aanmelden bij Experience Cloud duurt langer dan een seconde.
* Nadat u een aangepaste tag aan een element hebt toegevoegd, kunnen er geen andere metagegevenswijzigingen meer worden doorgevoerd.
* [!DNL Adobe Media Optimizer] maakt niet automatisch gebruikers wanneer de gebruiker is gemaakt in Experience Cloud.
* Opties in keuzelijsten met invoervak voor het tijdelijk toevoegen van nieuwe gebruikers verdwijnen tijdens het typen.
* Gegevens die worden gedeeld vanuit [!DNL Media Optimizer] Experience Cloud zijn onjuist vertegenwoordigd.
* Het delen van Flickr-afbeeldingen mislukt.
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in Experience Cloud.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* [!DNL Search&Promote] koppelingen zijn niet beschikbaar in [!UICONTROL organisaties en producttoegang].
* De gebruiker moet het bord vernieuwen om de verwijderde kaarten uit de weergave te laten verdwijnen.
* Sommige Excel- of CSV-bestanden kunnen niet naar een board worden geüpload.
* [!DNL Adobe Media Optimizer] simulatiekaarten worden niet correct weergegeven.
* Sommige PNG-bestanden kunnen niet op een kaart worden gerenderd.
* Bètafeedback kan niet worden verzonden.

## Release 14.2.1 - 24 februari 2014 {#section_5AD81B0737C843AFB4BE9C4420D70EB3}

<table id="table_DFAB002358C94A17A7F91DAB323A488F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Functie </th> 
   <th colname="col2" class="entry"> Beschrijving </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>OEmbed </p> </td> 
   <td colname="col2"> <p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Gegevens vernieuwen </p> </td> 
   <td colname="col2"> <p> 
     <!--MAC-18174-->Het pictogram Gegevens <span class="uicontrol"></span> vernieuwen voor een grafiek op een kaart is nu verborgen als de oplossing het vernieuwen van gegevens niet toestaat. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waardoor gedeelde [!DNL Analytics] rapporten geen segmentfilters konden toepassen.
* Probleem verholpen waarbij oplossingen als gekoppeld worden weergegeven op de pagina [!UICONTROL Experience Cloud Solutions] , zelfs als de accounts van de oplossingen niet gekoppeld waren.
* Probleem verholpen waarbij [!DNL Adobe Target] klanten in Azië niet op de knop **[!UICONTROL Doorgaan naar cloud]** op de koppelingspagina konden klikken.
* Probleem opgelost waarbij het delen van YouTube-video&#39;s werd voorkomen.
