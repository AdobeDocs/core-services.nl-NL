---
description: Hoe u Experience Cloud Triggers configureert.
keywords: integrations;Triggers
seo-description: Hoe u Experience Cloud Triggers configureert.
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Triggers

## Overzicht van triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

*Triggers* laten u toe om, zeer belangrijk consumentengedrag te identificeren te bepalen en te controleren, en dan dwars-oplossing mededeling te produceren om bezoekers opnieuw in dienst te nemen. U kunt triggers gebruiken in realtime beslissingen en personalisatie.

* Snel opnieuw op de markt brengen voor winkels met winkelwagentjes of winkels met winkels met winkels met winkels en winkels met verwijderde producten configureren
* Incomplete formulieren en toepassingen
* Handelingen of reeksen handelingen op de site

![](assets/trigger-abandonment-2.png)

**Typen triggers**

Over het algemeen kan het 15 tot 90 minuten duren voordat een marketingcampagne wordt gestart. Dit hangt van de implementatie van gegevensinzameling, lading op de pijpleiding, douaneconfiguratie van de bepaalde trekker, en het werkschema in de Campagne van Adobe af.

* **Afschaffing:** U kunt een trigger maken die moet worden geactiveerd wanneer een bezoeker een product weergeeft, maar er niets aan toevoegt. Configureer [Propensiteitscores](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334) om de neiging van klanten om niet te begrijpen na het verlaten van een winkelwagentje.
* **Handeling:** U kunt bijvoorbeeld triggers maken om na aanmelding voor nieuwsbrieven, e-mailabonnementen of aanvragen voor creditcards (bevestigingen) te activeren. Als u een detailhandelaar bent, kunt u een trekker voor een bezoeker tot stand brengen die zich voor een loyaliteitsprogramma ondertekent. In media en vermaak, creeer trekkers voor bezoekers die op een bepaalde show letten, en misschien wilt u met een onderzoek antwoorden.
* **Begin en einde sessie:** Maak een trigger voor het starten en beëindigen van de sessie.

## Een Experience Cloud-trigger maken {#task_821F37183AC045E5AC8EED20317598FE}

Maak een activeringstrigger en configureer de voorwaarden voor de trigger- en eigenschapscoring. U kunt bijvoorbeeld de criteria voor de regels van een trigger tijdens een bezoek opgeven, zoals maateenheden zoals Kart Abandon of afmetingen zoals de productnaam. Wanneer aan de regels wordt voldaan, loopt de trekker.

<!-- t_create-trigger.xml -->

>[!NOTE]
>
>Er bestaat momenteel een technische limiet van 100 triggers.

1. Klik in de Experience Cloud op ![](assets/menu-icon.png)en klik op **[!UICONTROL Activation]**.
1. Zoek de [!UICONTROL Triggers] kaart en klik op **[!UICONTROL Launch]**.

   ![Stap resultaat](assets/activation-triggers.png)

1. Klik **[!UICONTROL New Trigger]** en geef vervolgens het type trigger op:

   ![Stap resultaat](assets/add-trigger.png)

1. Vorm de trekker door de volgende gebieden te voltooien en metriek en afmetingspunten aan de containers van de regel te slepen:

   | Element | Beschrijving |
   |--- |--- |
   | Naam | De vriendelijke naam voor deze trigger. |
   | Beschrijving | De beschrijving van deze trigger, hoe u deze gaat gebruiken enzovoort. |
   | Rapportsuite | De [rapportsuite](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html) Analytics die voor deze trigger wordt gebruikt. Deze instelling identificeert de te gebruiken rapportgegevens. |
   | Bezoek moet<br>includeVisit mag geen<br>includeTrigger zijn na geen<br>actionInclusief metagegevens | U kunt criteria of gedrag van bezoekers bepalen die u wilt voorkomen, en gedrag dat u niet wilt voorkomen.  De regels voor een eenvoudige activering van een winkelwagentje kunnen bijvoorbeeld als volgt zijn:<ul><li>Het bezoek moet het volgende omvatten:  Kart optellen (metrisch) en bestaat. (U kunt de regel verder verfijnen met een specifieke productweergave of met afmetingen zoals Browsertypen.)</li><li>Bezoek mag niet omvatten:  Afhandeling.</li><li>Trigger na geen actie voor:  10 minuten.</li><li>Inclusief metagegevens: Hiermee kunt u een bepaalde dimensie of variabelen toevoegen die relevant zijn voor het gedrag van een bezoeker. Dit veld kan handig zijn voor Adobe Campaign om de juiste e-mail voor opnieuw marketing te maken.</li></ul><br>U kunt om het even welk, en of logica binnen of tussen containers specificeren, afhankelijk van de criteria u belangrijk voor de regel bepaalt. |
   | Container | In containers kunt u regels, voorwaarden of filters instellen en opslaan die een trigger definiëren. Als u wilt dat gebeurtenissen tegelijkertijd plaatsvinden, plaatst u ze in dezelfde container. Met andere woorden, elke container verwerkt onafhankelijk op raakniveau.  Bijvoorbeeld, als u twee containers hebt die door de exploitant worden aangesloten van En, kunt u de regels verwachten om te kwalificeren wanneer twee klappen aan de vereisten voldoen. |
   | Nieuwe sessie starten na | Maak een trigger voor het starten en beëindigen van de sessie. |

1. (Optioneel) In hechtenistriggers kunt u [Propensiteitscores](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334)toepassen.

   ![Stap resultaat](assets/propensity-scoring.png)

1. Klik op **[!UICONTROL Save]**.
1. Gebruik triggers voor [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Voorbeeld triggers

**Trigger voor weglating van winkelwagentje**

De volgende pagina bevat bijvoorbeeld regels die u kunt gebruiken voor een trigger voor het afbreken van winkelwagentjes, op basis van producten die tijdens een bezoek worden weergegeven.

![](assets/abandonment-trigger.png)

**Referrer Trigger**

De volgende trigger wordt geactiveerd wanneer een treffer wordt geleverd met het product van Men&#39;s Boots en referentie van Facebook. Om de twee criteria ( *producten* en *referentie*) in dezelfde hit te kunnen beoordelen, moeten ze aan dezelfde recipiënt worden toegevoegd.

![](assets/fb-boots-promo.png)

## Score volheid {#concept_A506150674AD45DB98D3CC07E560D334}

<!-- propensity-scoring.xml -->

Begrijp de neiging van klanten terug te keren na het verlaten van een winkelwagentje. Propensiteitsscoring is ingebouwd in Experience Cloud-triggers en is beschikbaar voor Abandenvironment-triggers.

![Stap resultaat](assets/propensity-scoring.png)

Sommige klanten verlaten bijvoorbeeld winkelwagentjes om gebruik te maken van e-mailprikkels om terug te keren naar het winkelwagentje. Om het inkomstenverlies te verminderen, helpt het Propensity Scoring algoritme de relevante kartondissidenten te identificeren die zonder de stimulans waarschijnlijk niet zouden terugkeren.

U kunt:

* Vermijd overmatige blootstelling van uw klanten aan re-marketing.
* Identificeer de juiste kar-verlaten klanten en kaart hun activiteit aan het juiste bericht.
* Verhoog de omzet door te weten welke klanten zullen en niet zullen terugkeren.

## De waarde van de waardestijging {#section_CA99874A25434CC0BF01D0DA61608889}

U kunt gegevensdetectie uitvoeren om verborgen gedragingen of patronen in uw gegevens te identificeren. Specifiek, helpt het bezit van de dichtheid die u clusters van gelijkaardige klanten identificeert gebruikend meer geconcentreerde en objectieve middelen eerder dan eenvoudige segmentatie of het filtreren. Bovendien laat het bezit u opstelling het voorspelbare mogelijkheden scoren om gedrag voor de hoge-waardeklant van uw bedrijf te identificeren.

Zodra u het hoogwaardigheidspubliek hebt geïdentificeerd, kunt u hen dan voor het grootste effect aanhalen. Bijvoorbeeld, als u zaken-aan-zaken bedrijf bent, kunt u verkoopvraaglood hebben die u toestaan om dan de lood te scoren en hun waarschijnlijkheid te identificeren om offline om te zetten. Omdat elke lead de kosten verhoogt, is het creëren van een prikkel om toekomstige klanten met de hoogste waarschijnlijkheid te identificeren van het omzetten van een verkoop de meest efficiënte en goedkoopste manier om uw middelen te concentreren.

Met de functie voor volheidsscoring kunt u de factoren identificeren die het meest voorspellend zijn voor een bepaalde score of de kans vergroten dat een gebeurtenis plaatsvindt, maar u kunt deze ook toepassen op het beantwoorden van specifieke vragen:

* Zal de klant converteren?
* Zal de klant op een e-mail antwoorden?
* Zal de klant terugkopen?

Met scoring in volheid kunt u deze vragen beantwoorden en bezoekers identificeren met een neiging tot actie die vervolgens kan worden ingesteld en gescoord.
