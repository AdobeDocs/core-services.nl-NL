---
description: '"Nieuwste functies, releaseopmerkingen en bekende problemen voor de Experience Cloud-services, zoals klantkenmerken, soorten publiek en gebruikersbeheer."'
keywords: kerndiensten
solution: Experience Cloud
title: 'Opmerkingen bij de cumulatieve release '
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
feature: '"Klantkenmerken"'
topic: Beheer
role: Administrator
level: Experienced
exl-id: b71d144c-a097-4cdb-9721-671519d38aff
source-git-commit: 55cbcc6663ca22bbcd13e76411433912d6132eed
workflow-type: tm+mt
source-wordcount: '4143'
ht-degree: 2%

---

# Opmerkingen bij de cumulatieve release

Functies, releaseopmerkingen en bekende problemen met de Experience Cloud Central Interface-componenten.

Zie [Experience Cloud](doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784) voor een lijst met documentatie-updates.

Zie [Opmerkingen bij de release Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=en) voor opmerkingen bij de release over alle oplossingen.

## Juni - 2021

| Functie | Datum | Beschrijving |
| ------- | ------- | ------- |
| Single Sign-On-ondersteuning voor Adobe-id&#39;s | 17 juni 2021 | Als u Federatieve id&#39;s gebruikt, kunt u zich aanmelden bij Experience Cloud zonder een e-mailadres of wachtwoord in te voeren. Als u deze functie wilt gebruiken, voegt u `#/sso:@domain` toe aan de URL van de Experience Cloud. <br>Stel dat u eigenaar bent van het domein  `adobecustomer.com` en u wilt aanmelden bij Adobe Analytics. De URL is: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`. |
| Experience League zoeken | 1 juni 2021 | Het zoeken naar documentatie van Experiencen League is verbeterd. Navigeer naar [Experience League](https://experienceleague.corp.adobe.com/docs/?lang=en) en gebruik het veld **[!UICONTROL Search]** om zelfstudies, documentatie, cursussen en meer te zoeken. |

{style=&quot;table-layout:auto&quot;}

## Mei - 2021

| Functie | Datum | Beschrijving |
| ------- | ------- | ------- |
| Experience Cloud-koptekst en -navigatie | 20 mei 2021 | Adobe Experience Cloud-updates bevatten een wijziging in het lichte thema voor de koptekst. U kunt gemakkelijk terugschakelen naar een donker thema en een koppeling maken om extra voorkeuren te bepalen vanuit de gebruikersavatar in de koptekst van de Experience Cloud. Hoewel niet alle toepassingen in Experience Cloud thema&#39;s ondersteunen, opent deze functie toekomstige themaondersteuning. |
| Experience Cloud Global Search | 20 mei 2021 | Met deze release kunt u met algemene zoekfunctie Experience Cloud zoeken in de documentatie, cursussen en zelfstudies van [Experience League](https://experienceleague.adobe.com/#home). (Momenteel is de algemene zoekopdracht alleen beschikbaar voor gebruikers in de Experience Platform. Met algemene zoekopdrachten naar [!UICONTROL Platform] kunt u zoeken naar elk bedrijfsobject in Experience Cloud, zoals segmenten, gegevenssets, schema&#39;s en meer.) |
| Voorkeuren voor Experience Cloud-taal | 20 mei 2021 | Deze update biedt de mogelijkheid om uw voorkeurstalen in te stellen in Experience Cloud [Voorkeuren](https://experience.adobe.com/preferences). |

{style=&quot;table-layout:auto&quot;}

## augustus - 2020

| Functie | Beschrijving |
| -----------| ---------- |
| Beheer - beleidsregels | Op deze pagina wordt een volledige lijst met beleid voor Experience Cloud in uw organisatie weergegeven. Het verstrekt informatie over producten, instanties, gebruikers, en ontwikkelaars. U kunt zoeken, sorteren en filteren op aangepaste weergaven van de lijst met beleidsregels. Zie [Help voor de Experience Cloud-beheertool](admin-tool-experience-cloud.md) voor meer informatie. |

{style=&quot;table-layout:auto&quot;}

## April - 2020

* De pagina Experience Cloud [!UICONTROL Feed] is afgeschaft. (EXC-8505)
* De aanmeldingspagina van Experience Cloud is bijgewerkt met nieuwe brandingselementen. (EXC-10747)

## februari - 2020

| Functie | Beschrijving |
| -----------| ---------- |
| Beheer - Gebruikersgegevens weergeven | Beheerders kunnen een sorteerbare en filterbare lijst met alle Experience Cloud-gebruikers en hun gegevens weergeven in het nieuwe Admin-gereedschap. De details van de gebruiker omvatten de het producttoegang van een gebruiker, rollen, en laatste betreden informatie. Zie [Help voor de Experience Cloud-beheertool](admin-tool-experience-cloud.md) voor meer informatie. |

{style=&quot;table-layout:auto&quot;}

**Oplossingen**

* **Klantkenmerken:gebruikersinterface** Klantkenmerken geeft nu aanvullende statussen weer van profielen die zijn gesynchroniseerd in Doel. (MCUI-10231)
* **Triggers Core Service:** wegens gebrek aan gebruik, is de &quot;Waarschijnlijkheid om binnen 30 dagen terug te keren&quot;van de neiging om een trekker van het type van Afschrijving te creëren verwijderd. (MCUI-10056)

## Januari - 2020

* De pagina &quot;Feed&quot; is in december 2019 vervangen. Zoek naar een bericht over afgekeurde producten. (MCUI-10039)

## Augustus - 2019

* Probleem verholpen waarbij een probleem met de aanmelding bij Experience Cloud werd opgelost dat ertoe leidde dat sommige gebruikers zich afmelden voor een sessie. (MCUI-6908)
* Bijgewerkte aanmelding van Experience Cloud om de prestaties te verbeteren en latentie te verminderen. (MCUI-6854, MCUI-6869, MCUI-6883)
* Bijgewerkte interface cosmetisch. (MCUI-6861, MCUI-6911, MCUI-6862)
* Probleem verholpen met Experience Cloud [!UICONTROL Triggers] die tot onjuiste interpretatie van _like_ clausule in de [!UICONTROL Trigger] definitie leidden. (MCUI-6611)

## April - 2019

* De app-schakeloptie is bijgewerkt zodat Marketo wordt opgenomen in de Experience Cloud-oplossingssuite en updates van de branding naar het Experience Platform. (MCUI-6529)
* Bijgewerkt startpunt Experience Cloud om navigatiekoppelingen naar de pagina&#39;s feed en beheer op te nemen. (MCUI-6682)
* Probleem opgelost in de [!UICONTROL Trigger]-definitie voor correct gebruik van de ‘like’-component. (MCUI-6611)
* Verbeteringen aan de Attributen van de Klant voor beter het registreren in de dienst van het Abonnement. (MCUI-6519)

## Release 19.1.1 - 17 januari 2019

**Opmerking:** In maart 2019 biedt de interface Experience Cloud geen ondersteuning voor Internet Explorer 11.

* Probleem verholpen waarbij het zoeken naar Help niet tot resultaten leidde. (MCUI-1670)
* Correctie en verbeterd beheer van eVar in Triggers. (MCUI-6400)

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
   <td colname="col1"> <p>Vooraf geconfigureerde productconfiguraties in de Admin Console </p> </td> 
   <td colname="col2"> <p>Klantenbeheerders van Experience Cloud kunnen productconfiguraties gebruiken die vooraf zijn gemaakt en zijn toegewezen aan standaardmachtigingsgroepen voor Analytics en Dynamic Tag Management. </p> <p>Deze optimalisatie is beschikbaar voor nieuwe provisioned organisaties, en het vermindert de hoeveelheid tijd die door organisaties wordt vereist om gebruikers in de Admin Console te beheren. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Voederverbetering </p> </td> 
   <td colname="col2"> <p> Wanneer het creëren van een post in de Diervoed van de Experience Cloud, gebruikt aan lijn nu het momenteel actieve onderwerp in plaats van het gebruiken van de organisatie door gebrek.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij miniaturen niet konden zien voor elementen die werden gedeeld van Assets op aanvraag naar de Experience Cloud-feed. (MAC-29955)

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
   <td colname="col1"> <p>Experience Cloud Elementen verbeteren </p> </td> 
   <td colname="col2"> <p>In Experience Cloud Assets kunt u uw digitale elementen opslaan, delen en synchroniseren vanaf één centrale locatie. Experience Cloud Assets gebruikt enkele functies die beschikbaar zijn in <span class="keyword"> Adobe Experience Manager</span> (AEM). </p> <p>Zie <a href="experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local"> Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verbeteringen voor het koppelen van accounts </p> </td> 
   <td colname="col2"> <p>Verbeterde interfacewerkstroom voor het verbinden van oplossingsrekeningen met de Experience Cloud (Adobe ID). Deze nieuwe workflow zoekt alle accounts van de gebruiker die aan een organisatie zijn gekoppeld en geeft u de mogelijkheid om te kiezen welk account aan een koppeling wordt gekoppeld. We hebben ook de koppelingservaring voor accounts gestroomlijnd, zodat u de pagina Organisaties beheren niet langer hoeft te openen om accounts handmatig te koppelen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij koppelingen en SSO voor Analytics werden voorkomen. Deze kwestie toonde de &quot;Bericht: Het foutbericht: FOUT IMS SSO is mislukt: Kan het gekoppelde bedrijf niet vinden.&quot;

**Bekend probleem**

Als u via de interface **[!UICONTROL Experience Cloud]** > **[!UICONTROL Activation]** toegang krijgt tot Dynamic Tag Management, maar uw Dynamic Tag Management-account is niet gekoppeld aan de Experience Cloud (Adobe ID), kunt u zich niet aanmelden bij Dynamic Tag Management. Navigeer rechtstreeks naar `dtm.adobe.com` in een nieuw browsertabblad om dit probleem te voorkomen.

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
>Microsoft® is [eindsteun](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) voor Internet Explorer 8, 9, en 10. Als zodanig, zullen wij geen kwesties bevestigen die tegen deze specifieke versies van Internet Explorer worden gemeld.

## Release 15.10 - 14 oktober 2015 {#section_68123833D3634BD3A473C12862BF9606}

**Bekende problemen**

* Klanten kunnen zich niet aanmelden bij Report Builder als ze zich via de Experience Cloud aanmelden bij Analytics. Dit probleem is niet van invloed op klanten die oude analysegegevens gebruiken.
* Bekende kwestie met de &quot;Verbinding aan de functie van het Rapport&quot;in Analytics. Klanten die zich via de Experience Cloud aanmelden bij Analytics, worden voor Analytics naar een niet-SSO-aanmeldingspagina geleid wanneer ze een rapport proberen te delen.

## Release 15.9 - 10 september 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Probleem met de prestaties van de Audience Manager-API die tot onderbrekingen leidden bij het uploaden van klantkenmerkgegevens, is opgelost. (MAC-26305)
* Probleem verholpen waarbij gebruikers maximaal 200 klantkenmerken aan een abonnement konden toevoegen. (MAC-26188)
* Probleem verholpen met Audience Library die ervoor zorgde dat het delen van het publiek niet werd beïnvloed door segmentering van Analytics. Dit probleem heeft ertoe geleid dat &quot;Gegevens verzamelen&quot; (0 soorten publiek) werd weergegeven. Om dit probleem te voorkomen, raadt Adobe aan de segmentgrootte onder de 50k van het publiek per segment te houden. (MAC-25788)
* Oplossing voor een eerder bekend probleem met de kenmerken van de klant - Bewerk de pagina Schema die een fout met behoud van inhoud veroorzaakte die werd gegenereerd bij het wijzigen van een weergavenaam. (MAC-25589, AN-103834)

## Release 15.7 - juli 2015 {#section_2683A152176944E48EF6C943892975B7}

* Probleem verholpen waardoor kenmerkbeschrijvingen die zijn opgegeven op de pagina Weergeven/Bewerken van schema (in Klantkenmerken) niet konden worden bijgewerkt in analyserapporten. (MAC-25985)
* Probleem verholpen waarbij de miniaturen niet konden worden gerenderd voor geüploade elementen. (MAC-25863)
* Probleem verholpen waardoor nieuwe segmenten die in rapporten en analyses zijn gemaakt, niet beschikbaar waren voor Experience Cloud-soorten publiek. (MAC-25817)
* Probleem verholpen waarbij delen van publiek door Analytics werd voorkomen bij gebruik van de service bezoekersidentiteitskaart. (MAC-25788, MAC-25747)
* Toegevoegde ondersteuning voor multibyte-tekens in klantkenmerken. (MAC-2552)

**Bekend probleem**

Een bekende kwestie veroorzaakt dubbele auto-geproduceerde rekeningen om in Audience Manager worden gecreeerd, en hen automatisch aan de identiteit van de Experience Cloud van een gebruiker te verbinden. Dit probleem doet zich voor als u naar de Audience Manager wilt navigeren voordat u uw accounts koppelt. Adobe raadt u aan uw Audience Manager-accounts aan de Experience Cloud te koppelen voordat u naar de Audience Manager navigeert. (MAC-25640)

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
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">De menuselecties <span class="term"> Audience Library</span> en <span class="term"> Customer Attributes</span> staan nu onder <span class="term"> Audiences</span>. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">De <span class="term"> Uitwisseling</span> menuselectie werd bewogen van het drop-down menu van de Hulp aan de linkernavigatiespoor. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> <span class="term"> </span> Oplossingen zijn verwijderd. U kunt alle oplossingen lanceren vanaf de onderste helft van de navigatieregel. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Probleem verholpen waarbij werd voorkomen dat klantkenmerken voor sommige klanten werden gesynchroniseerd.
* Probleem verholpen waarbij de pagina [Adobe Target-productdocumentatie](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=en) niet in het Japans kon worden weergegeven.
* Probleem verholpen waarbij het gebruik van Japanse tekst in opmerkingen tussen [!DNL Creative Cloud] en [!DNL Experience Cloud] werd voorkomen.

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
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Ondersteuning voor bedrijven en Federated ID </li> 
    </ul> </td> 
   <td colname="col2"> <p>De gebruiker en de functionaliteit van het groepsbeheer is verplaatst naar de Admin Console. Het nieuwe navigatiepad is: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt;  <span class="uicontrol"> Beheer</span>  &gt; Admin Console  <span class="uicontrol"> starten</span></p> <p> Er is ook ondersteuning toegevoegd voor bedrijfs- en gefedereerde id's. U kunt onderneming-id's, gefedereerde id's en Adobe-id's gebruiken in dezelfde implementatie voor de onderneming. Gebruik bijvoorbeeld Adobe-id's voor gebruikers die andere Adobe-producten en -services kunnen gebruiken. Gebruik bedrijf- of gefedereerde id's voor gebruikers waar u hun accounts strikt wilt beheren. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waarbij Single Sign-On tussen [!DNL Experience Cloud] en [!DNL Media Optimizer] werd voorkomen.

**Bekende problemen**

* Het koppelen en ontkoppelen van uw dynamische organisatie voor tagbeheer aan de Experience Cloud werkt niet voor nieuwe Experience Cloud-organisaties. Adobe werkt eraan dit probleem op te lossen en de normale functionaliteit te herstellen met de release van mei. Als u problemen ondervindt bij het aanmelden bij dynamisch tagbeheer via de Experience Cloud, gebruikt u de oudere aanmelding op [!DNL dtm.adobe.com].
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
   <td colname="col2"> <p>Als u gegevens van ondernemingsklanten in een gegevensbestand van het het relatiebeheer van de klant (CRM) vangt, kunt u de gegevens in een gegevensbron van de Attributen van de Klant in de Experience Cloud uploaden. Nadat de gegevens zijn geüpload, kunt u <span class="uicontrol"> Bezoekersprofiel</span> &gt; <span class="uicontrol"> Klantkenmerken</span> rapporten uitvoeren in Analytics. </p> <p>U kunt de geüploade gegevens ook gebruiken als een publiekssegment in <span class="keyword"> Adobe Target</span>. </p> <p>Zie <a href="attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1" format="dita" scope="local"> Klantkenmerken</a> productdocumentatie. </p> <p> Voor informatie over het moderniseren van uw oplossingen voor de kerndiensten, zie <a href="core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> uw oplossingen voor kerndiensten toelaten</a>. </p> </td> 
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
   <td colname="col2"> <p>De pagina van het Beheer van de Groep is herontworpen als administratieve interface die u groepen laat tot stand brengen, gebruikers aan groepen toevoegen, en toestemmingen over de oplossingen van Experience Cloud toepassen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Toewijzing van één naar veel </p> </td> 
   <td colname="col2"> <p>Wanneer het verbinden van oplossingsrekeningen in de Experience Cloud, als u veelvoudige oplossingen en organisaties hebt, kunt u veelvoudige producten en de diensten aan één enkele organisatie nu in kaart brengen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activering </p> </td> 
   <td colname="col2"> <p> <a href="activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local"> </a> Activering wordt nu weergegeven in de linkernavigatie in de  <span class="keyword"> Experience Cloud</span>. <span class="wintitle"> </span> Activation is een  <span class="keyword"> Experience </span> Cloudservice die momenteel bestaat uit de technologie voor dynamisch tagbeheer en geeft u de leiding wanneer u erop klikt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Documentatie-updates - Core Services </p> </td> 
   <td colname="col2"> <p>Het onderwerp <a href="core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Uw oplossingen voor kernservices inschakelen</a> is toegevoegd om u te helpen bij de implementatie van kernservices. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Release 15.2.1 - 19 februari 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Oplossingen:

* Verbeterde werkstroom voor e-mailuitnodigingen van gebruikers voor het instellen van accounts.
* Probleem verholpen met een elementmap waardoor [!DNL Experience Cloud]- en [!DNL Adobe Campaign]-elementen geen identieke maphiërarchieën konden weergeven.
* Probleem verholpen waarbij het verwijderen van soorten publiek die deel uitmaakten van gedeactiveerde [!DNL Target]-activiteiten werd voorkomen.
* Probleem verholpen waarbij het pictogram Toevoegen (plus) niet onder [!UICONTROL Rules] op de pagina [!UICONTROL Create New Audience] kon worden weergegeven.
* Verbeterde ondersteuning voor de Experience Cloud-interface voor Internet Explorer 9.

## Release 15.1.1 - 15 januari 2015 {#section_F1A352E928AF432E94CC0A289C345184}

Nieuwe eigenschappen en moeilijke situaties in [!DNL Adobe Experience Cloud] samenwerking en het delen interface.

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
* De gebruikers zouden verbindingen op hun Experience Cloud kaarten van Media Optimizer kunnen missen.
* Sommige administratieve gebruikers zouden kwesties kunnen ervaren die hun rekeningen verbinden na het goedkeuren van een uitnodiging om zich bij de Experience Cloud aan te sluiten.
* De Experience Cloud-interface kan de prestaties verminderen wanneer deze gelijktijdig door meerdere gebruikers wordt gebruikt.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Sommige gebruikers kunnen problemen ondervinden wanneer ze zich gelijktijdig aanmelden bij twee browsers met dezelfde Adobe ID.
* Sommige gebruikers kunnen een gebruiker van de Creative Cloud aan een gedeelde omslag niet opnieuw toevoegen nadat de gebruiker van de Creative Cloud is geschrapt.
* Sommige gebruikers ondervinden mogelijk een vertraging in het bericht dat optreedt wanneer een map wordt gedeeld van de Experience Cloud naar de Creative Cloud.
* Sommige gebruikers kunnen problemen ondervinden bij het delen van een map tussen de Experience Cloud en de Creative Cloud.
* Sommige gebruikers kunnen problemen ondervinden bij het maken van een publiek in een Analytics-rapportensuite nadat het gedeelde publiek is ingeschakeld.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.

## Release 14.11.1 - 13 november 2014 {#section_A6CF1D4F27B9496892A89C983EB39102}

Bekende problemen:

* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden gerenderd.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Beheerders moeten zich afmelden en weer aanmelden om de wijzigingen te kunnen zien die in Accountinstellingen zijn aangebracht.
* Gebruikers kunnen PowerPoint-bestanden niet delen op borden.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* Synchronisatie tussen Adobe Experience Manager en Creative Cloud werkt niet.

## Release 14.10.1 - 16 oktober 2014 {#section_E3A0F4423B814707AA3745E083500835}

Nieuwe eigenschappen en moeilijke situaties in [!DNL Adobe Experience Cloud] samenwerking en het delen interface.

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
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">Klik op <span class="uicontrol"> Instellingen</span> in het bord. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Geef <span class="uicontrol"> Eigenaar</span>, <span class="uicontrol"> Viewer</span> of <span class="uicontrol"> Editor</span> naast elke eigenaar op. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Er werd een foutbericht geretourneerd wanneer u een kaart maakte van een PDF en deze naar het bord deelde.

**Bekende problemen**

* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden gerenderd.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Gebruikers kunnen PowerPoint-bestanden niet delen op borden.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De koppeling [!DNL Search&Promote] is niet beschikbaar op de pagina [!UICONTROL Organizations & Product Access].

## Release 14.9.1 - 18 september 2014 {#section_20F156A9CC2F4FC59C4970075C181D3A}

**Oplossingen en verbeteringen**

* Wanneer u aan [!DNL experience.adobe.com] navigeert, is de login ervaring nu verenigbaar met login van Adobe Creative Cloud.
* Op de pagina Organisaties beheren is de koppelingservaring (nadat een uitnodiging is ontvangen) nu consistent voor elke oplossing.

**Bekende problemen**

* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Gebruikers kunnen PowerPoint-bestanden niet delen op borden.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden gerenderd.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De koppeling [!DNL Search&Promote] is niet beschikbaar op de pagina [!UICONTROL Organizations & Product Access].
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud]-inhoud uit hun map wordt verwijderd als de inhoud niet wordt gedeeld in [!DNL Experience Cloud].

## Release 14.8.1 - augustus 2014 {#section_03BF00F6A95A490C91BCC0A1988FA7AA}

Nieuwe eigenschappen en moeilijke situaties in [!DNL Adobe Experience Cloud] samenwerking en het delen interface.

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
   <td colname="col2"> <p>U kunt <span class="keyword"> de Mobiele Diensten van de Adobe nu tot</span> van de linkernavigatie toegang hebben. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekende problemen**

* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* Sommige gebruikers kunnen geen kaart maken van een PDF en deze delen naar een kaart.
* Sommige gebruikers kunnen problemen hebben met het uploaden van middelen naar een board.
* Sommige gebruikers kunnen zich mogelijk niet aanmelden van [!DNL Target] tot [!DNL Experience Cloud].
* Sommige gebruikers van Audience Managers kunnen zich niet aanmelden bij [!DNL Experience Cloud].
* Sommige gebruikers kunnen een verouderd element verwijderen in plaats van een foutmelding te ontvangen.
* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* Gebruikers kunnen PowerPoint-bestanden niet delen op borden.
* Sommige [!DNL .png] bestanden kunnen niet op een kaart worden gerenderd.
* [!DNL Experience Cloud] de interface kan prestaties verminderen wanneer in parallel gebruik door vele gebruikers.
* De koppeling [!DNL Search&Promote] is niet beschikbaar op de pagina [!UICONTROL Organizations & Product Access].
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud]-inhoud uit hun map wordt verwijderd als de inhoud niet wordt gedeeld in [!DNL Experience Cloud].

## Release 14.7.1 - juli 2014 {#section_B22D4F830756463DB27BB4D508D9ADD5}

Nieuwe eigenschappen en moeilijke situaties in [!DNL Adobe Experience Cloud] samenwerking en het delen interface.

**Bekende problemen**

* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* Sommige [!UICONTROL Exchange] gebruikers vinden hun namen in de commentaren misschien een lange koord ID in plaats van hun namen
* Sommige [!DNL .png]-bestanden kunnen niet op een kaart worden gerenderd
* Bij het uploaden van bestanden zijn meer bestandstypen toegestaan dan bij slepen en neerzetten. Upload voor de beste resultaten met [!UICONTROL Assets].
* De koppeling [!DNL Search&Promote] is niet beschikbaar op de pagina [!UICONTROL Organizations & Product Access].
* [!DNL Exchange] gebruikers moeten hun cookies wissen om hun ervaring te verbeteren.
* [!DNL Experience Cloud] de interface kan vertragen wanneer in parallel gebruik door vele gebruikers.
* Sommige gebruikers kunnen ervaren dat hun [!DNL Creative Cloud]-inhoud uit hun map wordt verwijderd als de inhoud niet wordt gedeeld in [!DNL Experience Cloud].
* U wordt afgemeld na 15 minuten inactiviteit. Ook, logout in één plaats meldt u uit [!DNL Experience Cloud].
* Sommige gebruikers kunnen hun Audience Manager-accounts mogelijk niet koppelen aan [!DNL Experience Cloud].
* [!UICONTROL Exchange] gebruikers kunnen alleen Engels zien in de taalkiezer.

**Oplossingen**

Geen om te rapporteren.

## Release 14.6.1 - 19 juni 2014 {#marketing_cloud_interface}

Nieuwe eigenschappen en moeilijke situaties in [!DNL Adobe Experience Cloud] samenwerking en het delen interface.

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
   <td colname="col1"> <p> <span class="wintitle"> Knop </span> Opslaan in publiek </p> </td> 
   <td colname="col2"> <p>Wanneer u een publiek creeert, wordt <span class="wintitle"> sparen</span> knoop op <span class="wintitle"> Create Nieuwe Publiek</span> pagina nu onbruikbaar gemaakt tot alle vereiste gebieden worden voltooid. 
     <!--MAC-19712 --></p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekende problemen**

* Bestanden die zijn verwijderd uit [!DNL Experience Cloud] worden niet verwijderd uit [!DNL Digital Asset Management].
* Bij het uploaden van bestanden zijn meer bestandstypen toegestaan dan bij slepen en neerzetten. Upload het bestand met Middelen voor de beste resultaten.
* De koppeling [!DNL Search&Promote] is niet beschikbaar op de pagina [!UICONTROL Organizations & Product Access].
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in [!DNL Experience Cloud].
* Sommige gebruikers kunnen hun account voor publieksbeheer niet koppelen aan hun [!DNL Experience Cloud]-account.
* U wordt afgemeld na 15 minuten inactiviteit. Ook, logout op één plaats meldt u uit de Experience Cloud.
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
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt;  <span class="uicontrol"> Help</span> &gt;  <span class="uicontrol"> Exchange</span></p> <p>De <span class="keyword"> Experience Cloud</span><span class="wintitle"> Uitwisseling</span> is één enkele bestemming waar u kunt zoeken, doorbladeren, selecteren, betalen, en downloaden digitale marketing uitbreidingen via apps. </p> <p>Apps omvatten schakelaars, douaneconfiguraties aan Adobe basisproduct, derdetoepassingen, rapporten, en <span class="keyword"> Experience Cloud</span> kaarten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud publiek </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt;  <span class="uicontrol"> Soorten publiek</span></p> <p> <span class="wintitle"> Het </span> publiek waar u creeert, uitgeeft, en beheert publiek, gelijkend op hoe u met segmenten werkt. Bijvoorbeeld, kunt u een segment in Rapporten &amp; Analytics tot stand brengen, dan het delen aan <span class="wintitle"> Experience Cloud</span><span class="wintitle"> Soorten publiek</span>. Zodra gedeeld, is het publiek beschikbaar in <span class="keyword"> Adobe Target</span> voor campagneactiviteiten, en in Adobe Audience Manager voor segmentatie. </p> <p> <p>Opmerking: Om activering in Doel te verzoeken, bezoek <a href="https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES" format="http" scope="external"> https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Gebruikers die op <span class="keyword"> Experience Cloud</span> kaarten worden vermeld hebben nu toestemmingen aan die kaart. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Nieuwe gebruikers van Adobe kunnen hun Scene7-accounts koppelen aan Adobe ID en hun teamleden. Beheerders kunnen gebruikers ook ontkoppelen van Scene7-accounts. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Asset-synchronisatie. </p> </td> 
   <td colname="col2"> <p> U kunt elementen binnen Experience Manager-elementen delen met Experience Cloud en Creative Cloud. Wijzigingen in deze elementen worden weerspiegeld in de gedeelde kopieën van de elementen in Experience Cloud en Creative Cloud. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* [!DNL Experience Cloud] was niet verbonden met  [!DNL Adobe Target]. Dit probleem is opgetreden als de [!DNL Adobe Target]-aanmelding op meerdere [!DNL Target]-servers kan worden gebruikt.
* [!DNL Adobe Media Optimizer] heeft niet automatisch gebruikers gemaakt wanneer de gebruiker is aangemaakt in  [!DNL Experience Cloud].
* Opties in keuzelijsten met invoervak die worden gebruikt voor het tijdelijk toevoegen van nieuwe gebruikers zijn tijdens het typen verdwenen.
* Er kan niet op de koppeling Opmerkingen in de weergave voor de kaart van het element worden geklikt.
* Nadat u een aangepaste tag aan een element hebt toegevoegd, zijn er geen andere metagegevenswijzigingen meer.
* Als u een afbeelding verwijdert, wordt er in Elementen niet gewaarschuwd of de afbeelding wordt gebruikt in Adobe Target Essentials.
* Trage [!UICONTROL Experience Cloud] interfaceprestaties bij parallel gebruik door veel gebruikers.
* Als u een afbeelding verwijdert in [!UICONTROL Experience Cloud Assets], verschijnt er geen waarschuwing als de afbeelding wordt gebruikt in [!DNL Adobe Target Essentials].
* Wanneer **[!UICONTROL remember me]** niet tijdens login werd geselecteerd, werd de gebruiker na 15 minuten het programma geopend.
* Gebruikers moesten zich afmelden en weer inloggen om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Aanmelden bij [!DNL Experience Cloud] duurde langer dan een seconde.
* Voor bepaalde gebruikers synchroniseerde het schrappen van dossiers van [!DNL Experience Cloud] niet met [!DNL Digital Asset Management].
* Gebruikers werden afgemeld na slechts 15 minuten browserinactiviteit.
* De gebruiker kon geen PowerPoint-bestanden op borden delen.
* Sommige gebruikers hadden een slechte visuele lay-out in Internet Explorer 10.

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
   <td colname="col2"> <p>Nadat u de functie Delen naar Adobe Experience Cloud hebt ingeschakeld op de werkbalk Bladwijzer van uw browser, kunt u nu Help-pagina's delen via de URL van de microsite. </p> <p> <b>Een Help-onderwerp delen</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Klik in <span class="keyword"> Experience Cloud</span> op <span class="uicontrol"> Beheer</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Sleep de knop <span class="uicontrol"> Delen naar Adobe Experience Cloud</span> naar de werkbalk Bladwijzer. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navigeer naar een Help-pagina (of blijf op deze pagina) en klik vervolgens op <span class="uicontrol"> Delen naar Adobe Experience Cloud</span> op de werkbalk Bladwijzers van uw browser. </p> <p>Deze stap leidt tot een kaart, die u in <span class="wintitle"> Experience Cloud </span> kunt bekijken. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Nadat u een aangepaste tag aan een element hebt toegevoegd, kunnen er geen andere metagegevenswijzigingen meer worden doorgevoerd.
* Gebruikers moeten het bord vernieuwen om de verwijderde kaarten uit het zicht te laten verdwijnen.
* Wanneer **[!UICONTROL Remember me]** niet is geselecteerd tijdens het aanmelden, wordt de gebruiker na 15 minuten afgemeld
* [!DNL Analytics] de openingspagina van de oplossing toont formatterende fouten.
* Gebruikers dienen zich af te melden en zich weer aan te melden om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Als u een afbeelding verwijdert, wordt [!UICONTROL Assets] niet gewaarschuwd of de afbeelding wordt gebruikt in [!DNL Adobe Target Essentials].
* Er kan niet op de koppeling Opmerkingen in de weergave met de elementenkaart worden geklikt.
* Opties in keuzelijsten met invoervak voor het tijdelijk toevoegen van nieuwe gebruikers verdwijnen tijdens het typen.
* Aanmelden bij [!DNL Experience Cloud] duurt langer dan een seconde.
* Gegevens die worden gedeeld vanuit [!DNL Media Optimizer] worden onjuist weergegeven in [!DNL Experience Cloud].
* Met Adobe [!DNL Media Optimizer] worden niet automatisch gebruikers gemaakt wanneer een gebruiker is gemaakt in [!DNL Experience Cloud].
* De [!DNL Experience Cloud] kan niet aan [!DNL Adobe Target] worden verbonden, als [!DNL Adobe Target] login op veelvoudige [!DNL Target] servers kan worden gebruikt.
* [!DNL Experience Cloud] de interface kan vertragen wanneer in parallel gebruik door vele gebruikers.
* [!DNL Search&Promote] koppeling is niet beschikbaar op de  [!UICONTROL Organizations & Product Access] pagina.
* [!DNL Adobe Media Optimizer] simulatiekaarten worden niet correct weergegeven.
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in [!DNL Experience Cloud].
* Filters die worden toegepast op trended-rapporten van Analytics worden niet toegepast op kaarten in Experience Cloud.
* Sommige Excel- of CSV-bestanden kunnen niet naar een board worden geüpload.
* Sommige gebruikers kunnen hun account voor publieksbeheer niet koppelen aan hun [!DNL Experience Cloud].
* Sommige gebruikers kunnen een fout ervaren bij het delen van [!DNL Analytics]-segmenten in [!DNL Experience Cloud].
* Sommige gebruikers kunnen mogelijk niet naar submappen gaan in [!UICONTROL Asset Selector].
* Sommige gebruikers kunnen geen gadgets voor AdLens delen in [!DNL Experience Cloud].

## Release 14.3.1 - 13 maart 2014 {#section_5D142E3225E3477A84DC01B8197D39BC}

Versie 14.3.1 is een onderhoudsversie die zich op snelheid, stabiliteit, en veiligheid concentreert. Belangrijke nieuwe functies worden niet opgenomen.

**Oplossingen**

* Hiermee kunt u uw avatar-afbeelding verwijderen.
* Probleem verholpen waarbij u uw [!DNL Adobe Media Optimizer]-accounts niet kon ontkoppelen.

**Bekende problemen**

* Als u een afbeelding verwijdert in Experience Cloud Assets, wordt niet gewaarschuwd of de afbeelding wordt gebruikt in Adobe Target Essentials.
* Het vernieuwen van een kaart van [!DNL Analytics] kan soms tot een leeg diagram in de uitgebreide kaart leiden.
* Gebruikers dienen zich af te melden en zich weer aan te melden om alle machtigingen en machtigingswijzigingen van kracht te laten worden.
* Wanneer *`Remember me`* niet tijdens login wordt geselecteerd, zal de gebruiker na 15 minuten worden het programma geopend.
* [!DNL Analytics] de openingspagina van de oplossing toont formatterende fouten.
* U kunt niet klikken op de koppeling Opmerkingen in de weergave met de elementenkaart.
* De Experience Cloud-interface kan vertragen wanneer veel gebruikers deze parallel gebruiken
* Experience Cloud kan niet worden gekoppeld aan [!DNL Adobe Target] als de [!DNL Adobe Target]-aanmelding kan worden gebruikt op meerdere doelservers.
* Aanmelden bij Experience Cloud duurt langer dan een seconde.
* Nadat u een aangepaste tag aan een element hebt toegevoegd, kunnen er geen andere metagegevenswijzigingen meer worden doorgevoerd.
* [!DNL Adobe Media Optimizer] maakt niet automatisch gebruikers wanneer de gebruiker in Experience Cloud is gemaakt.
* Opties in keuzelijsten met invoervak voor het tijdelijk toevoegen van nieuwe gebruikers verdwijnen tijdens het typen.
* Gegevens die worden gedeeld vanuit [!DNL Media Optimizer] zijn onjuist vertegenwoordigd in Experience Cloud.
* Het delen van Flickr-afbeeldingen mislukt.
* Filters die worden toegepast op trended-rapporten van [!DNL Analytics] worden niet toegepast op kaarten in Experience Cloud.
* Wijzigingen in groep- en machtigingen die zijn aangebracht in gebruikersbeheer, worden pas na een nieuwe aanmelding van kracht.
* [!DNL Search&Promote] koppelen is niet beschikbaar vanuit  [!UICONTROL Organizations & Product Access].
* Gebruikers moeten het bord vernieuwen om de verwijderde kaarten uit het zicht te laten verdwijnen.
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
     <!--MAC-18174-->Het pictogram  <span class="uicontrol"> Gegevens </span> vernieuwen voor een grafiek op een kaart is nu verborgen als de oplossing het vernieuwen van gegevens niet toestaat. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Oplossingen**

* Probleem verholpen waardoor gedeelde [!DNL Analytics]-rapporten geen segmentfilters konden toepassen.
* Probleem verholpen waarbij oplossingen als gekoppeld op de pagina [!UICONTROL Experience Cloud Solutions] worden weergegeven, zelfs als de accounts van de oplossingen niet zijn gekoppeld.
* Probleem verholpen waardoor klanten in Azië [!DNL Adobe Target] niet op de koppelingspagina op de knop **[!UICONTROL Continue to Experience Cloud]** konden klikken.
* Probleem opgelost waarbij het delen van YouTube-video&#39;s werd voorkomen.
