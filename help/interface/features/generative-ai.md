---
title: Generatieve AI in Experience Cloud-toepassingen
description: Ontdek meer over generatieve AI (GenAI) en hoe Experience Cloud-applicaties gebruikmaken van GenAI en [!UICONTROL AI Assistant].
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 2e8ce339aaf3d90b7ee6da2cdec1565c88513e3d
workflow-type: tm+mt
source-wordcount: '1753'
ht-degree: 3%

---

# Generatieve AI in Experience Cloud-producten

Met Generative AI (genAI) in Experience Cloud kunt u creatieve en cognitieve taken automatiseren en de productiviteit verhogen. Deze pagina beschrijft waar Experience Cloud-toepassingen genAI en AI Assistant ondersteunen en bevat koppelingen voor meer informatie over deze functies.

**wat is genAI?**

Generatieve AI is een type AI die originele inhoud kan maken. Zo kunt u bijvoorbeeld tekst, afbeeldingen, video, audio of softwarecode maken als reactie op een vraag of verzoek van een gebruiker.

* **creeer:** de capaciteit om inhoud (tekst, beelden, muziek, of video&#39;s) van kras te produceren, die op zijn opleiding en inputherinneringen wordt gebaseerd. Dit vermogen is het _generatieve_ aspect van generatieve AI.

* **produceer een reactie:** AI verstrekt een antwoord of een reactie op een herinnering, typisch trekkend op zijn beschikbare gegevens en kennisbewaarplaatsen.

**wat is [!UICONTROL AI Assistant]?**

[!UICONTROL AI Assistant] is een conversatiegereedschap dat wordt ondersteund in Experience Platform en verwante toepassingen. Gebruik het om _productkennis_ en _operationele inzichten_ in gesteunde producten snel te bereiken.

* **de kennis van het Product:** de kennis van het Product verwijst naar concepten en onderwerpen die in de documentatie van Experience League worden gegrond. Leer hoe te om efficiënte, [ op doelstelling-gebaseerde herinneringen ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/home) tot stand te brengen om het meeste uit [!UICONTROL AI Assistant] te krijgen. Alle antwoorden van Experience League zijn controleerbaar en worden met links genoemd.

* **Operationele inzichten:** [ Operationele inzichten ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/questions#objects-questions) verwijzen naar geproduceerde reacties over uw meta-gegevensvoorwerpen (attributen, publiek, dataflows, datasets, etc.). Met [!UICONTROL AI Assistant] kunt u in seconden bereiken wat anders uren of dagen kan duren.

De Medewerker van AI omvat ook de eigenschappen van gespreksagent AI (die als _worden bekend agentic AI_) in gesteunde toepassingen:

* **de steun van het Product:** de [ Agent van de Steun van het Product ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/new-features/customer-support) is het zelf-dienen het zuiveren en het oplossen van problemenvermogen van [!UICONTROL AI Assistant] dat u voor de eigenschappen en toepassingen van Experience Platform kunt gebruiken. Los steunkwesties op zonder uw werkschema te verlaten, creeer klantensteunkaartjes, en spoorcase progress gebruikend AI Medewerker.

[ Leer over Medewerker AI ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/landing)

## beschikbaarheid van GenAI in Experience Cloud-producten {#products}

De volgende Experience Cloud-toepassingen ondersteunen generatieve AI of [!UICONTROL AI Assistant] . Ondersteuning voor Adobe Firefly wordt ook per product aangegeven.

Bijgewerkt: **9 Juni, 2025**

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager]](#aem)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] Beheerde cloudservices](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] is een generatieve AI-toepassing die is ontworpen om marketingteams van bedrijven te helpen bij het maken, activeren en optimaliseren van campagneinhoud van het merk op verschillende kanalen, zoals betaalde media, e-mail en weergaveadvertenties.

Prestatiemarkeringen kunnen natuurlijke taalaanwijzingen gebruiken om gepersonaliseerde, merkconforme middelen te genereren. GenStudio for Performance Marketing versnelt de uitvoering van de campagne, schaalt de productie van inhoud zonder de integriteit van het merk in het gedrang te brengen, en biedt prestatieanalyses voor het verbeteren van het totale investeringsrendement.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

De verenigbaarheid van Adobe Firefly: **ja**

## [!DNL Experience Manager] {#aem}

In de volgende secties wordt een korte beschrijving gegeven van generatieve AI in AEM-toepassingen.

### Experience Manager Sites

In AEM Sites kunt u _[!UICONTROL Generate Variations]_&#x200B;gebruiken. Deze functie gebruikt generatieve kunstmatige intelligentie om inhoudvariaties te creëren die op uw inputherinneringen worden gebaseerd. Prompts worden geleverd door Adobe of gemaakt en beheerd door u.

Na het creëren van variaties, kunt u de inhoud op uw website gebruiken en zijn succes meten gebruikend de [ eigenschap van de Experimentatie ](https://www.aem.live/docs/experimentation) in Edge Delivery Services. U kunt ook afbeeldingen genereren in Adobe Express met behulp van de generatieve AI-mogelijkheden van Firefly.

**Input en outputvoorbeelden**

Invoervelden zijn:

* Aantal te genereren variaties
* Publiek Source
* Doelgroep publiek
* Aanvullende context
* Door de klant gestuurde vragen

De output is geproduceerde inhoud of marktexemplaar.

De verenigbaarheid van Adobe Firefly: **ja**

[Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

### Sites Optimizer {#sites-optimizer}

AEM Sites Optimizer gebruikt generatieve AI om de prestaties en effectiviteit van webervaringen te analyseren en te verbeteren. Deze inzichten worden gegroepeerd in belangrijke opportuniteitsgebieden: Betrokkenheid, Verkeersverwerving, Beveiligingstelling en, Sitegezondheid. Elke categorie benadrukt specifieke manieren om uw plaats te verbeteren, hetzij door bezoekersinteractie te verhogen, ontdekkingsbaarheid te verbeteren, veiligheid te versterken, of plaatsstabiliteit te handhaven. [Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-manager-sites-optimizer/content/opportunity-types/overview)

### Experience Manager Assets {#aem-assets}

In AEM Assets, kunt u generatieve AI in **Content Hub** gebruiken en **AI-Gegenereerde Slimme Markeringen**.

De verenigbaarheid van Adobe Firefly: **ja**

**Content Hub**

[!UICONTROL Content Hub] is beschikbaar als onderdeel van [!DNL Experience Manager Assets as a Cloud Service] voor het democratiseren van de toegang tot online-inhoud voor organisaties en hun zakelijke partners. Het richt zich op het distribueren van middelen voor activering op schaal en het creëren van varianten van on-brand-inhoud met het oog op verbeterde marketingflexibiliteit.

In Content Hub kunt u inhoud maken met Adobe Express (als u Adobe Express-rechten hebt). U kunt bestaande inhoud bewerken met eenvoudige gereedschappen, merkvariaties produceren met sjablonen en merkelementen en inhoud maken met de nieuwste GenAI-mogelijkheden van [!DNL Adobe Firefly] . [Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview)

**Slimme Markeringen**

In plaats van handmatig in te voeren, kan AI automatisch beschrijvende tags toewijzen aan digitale elementen. Deze door AI gegenereerde tags verbeteren de kwaliteit van de metagegevens, waardoor de elementen gemakkelijker kunnen worden doorzocht, gecategoriseerd en aanbevolen.

Als het element bijvoorbeeld een afbeelding is, kan AI objecten, scènes, emoties of zelfs merklogo&#39;s identificeren. Het kan relevante markeringen zoals _zonsondergang_, _strand_, _vakantie_, of _het glimlachen_ produceren. [Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/assets/manage/smart-tags#ai-smart-tags)

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO), kunt u [ AI Medewerker ](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/get-started/ai-assistant) gebruiken om _productkennis_ en _operationele inzichten_ (bèta) te bereiken.

### Voorbeelden van het gebruik van AI Assistant in AJO

Hier volgt een voorbeeldinput voor productkennis:

* _Hoeveel levende activiteiten kan ik in één zandbak van Journey Optimizer hebben?_

  De uitvoer wordt gegenereerd vanuit Experience League en andere Adobe-gegevensopslagruimten.

Hier volgt een voorbeeldinput voor operationele inzichten:

* _hoeveel Reizen in de laatste zeven dagen zijn gecreeerd?_

  Voor output, vraagt de Medewerker van AI een klant-specifieke gegevensopslag. De gegevensopslag bevat gecentraliseerde, operationele gegevens over [!UICONTROL Journeys]. Deze functie is onduidelijk voor de klant en haalt alleen metagegevens van zakelijke objecten op. Er worden geen gegevens in uw sandbox geopend.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/get-started/ai-assistant)

De verenigbaarheid van Adobe Firefly: **Nr**

### AI Assistant voor het genereren van inhoud (AJO Prime en Ultimate) {#ajo-prime}

In AJO _Prime_ en _Ultimate_, kunt u [ inhoudsgeneratie ](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) voor inhoudsgeneratie gebruiken om pro-actieve suggesties van de inhoudsvariatie voor tekst en beelden te brengen.

Deze functie is beschikbaar voor e-mail, pushberichten, webpagina&#39;s, inhoud en SMS-kanalen. Deze biedt snel gebaseerde tekst en het genereren van afbeeldingen. Uitvoer van het genereren van inhoud in AJO Prime en Ultimate is gegarandeerd.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

De verenigbaarheid van Adobe Firefly: **ja**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B edition gebruikt [!UICONTROL AI Assistant] om u te helpen met productkennis.

Voorbeeld-invoer:

* _hoe ik een e-mail in een rekeningsreis verzend?_

  De uitvoer van productkennis wordt vanuit Experience League opgehaald.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Campaign] Beheerde cloudservices {#campaign-cs}

Met Campagne Managed Cloud Services wordt [!UICONTROL AI Assistant] gebruikt voor het genereren van inhoud. Met deze functie kunt u automatisch gepersonaliseerde, aantrekkelijke en effectieve inhoud genereren op basis van uw marketingdoelstelling, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, tinten en meer met een merknaam. U kunt het gebruiken over kanalen zoals e-mail, SMS, en duw.

**Nota:** de Output van inhoudsgeneratie in de Beheerde Diensten van de Wolk van de Campagne wordt bevestigd.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/campaign-web/v8/content/ai-assistant/generative-gs)

De verenigbaarheid van Adobe Firefly: **ja**

## [!DNL Customer Journey Analytics] {#cja}

Met Customer Journey Analytics kunt u op de volgende manieren generatieve AI of AI Assistant gebruiken:

* [ AI Medewerker ](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) voor productkennis.
* [ Agent van de Steun van het Product ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/new-features/customer-support) om de kaartjes van de klantensteun, volledig met context en zittingsdetails van uw interactie met AI Medewerker tot stand te brengen.
* [ de Agent van Gegevens van Inzichten ](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) voor antwoorden op vragen over uw gegevens. In Analysis Workspace worden relevante visualisaties gemaakt aan de hand van componenten uit uw gegevensweergave en met behulp van uw werkelijke gegevens.
* [ Intelligente Bijschriften ](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) om zeer belangrijke inzichten voor de vaakst gebruikte Workspace visualisaties in natuurlijke taal te verstrekken.
* [ Content Analytics ](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/content-analytics/report/report#template) om elk activa automatisch meta-gegevens toe te wijzen.

De verenigbaarheid van Adobe Firefly: **Nr**

**AI Medewerker**

Ontdek productkennis van Experience League. Als u een nieuwe gebruiker bent, leert u snel de concepten van Customer Journey Analytics en neemt u uzelf op voor producten en functies. Bijvoorbeeld:

* _hoe ik een e-mail in een rekeningsreis verzend?_

Ervaren gebruikers krijgen geavanceerde gebruiksgevallen of leren strategieën om taken snel uit te voeren. U kunt concepten snel begrijpen, problemen oplossen, of naar informatie zoeken.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

**Intelligente Bijschriften**

U kunt _Intelligente Bijschriften_ in [!DNL Customer Journey Analytics] gebruiken om natuurlijk-taalinzichten voor de het vaakst gebruikte Workspace visualisaties te krijgen. Intelligente bijschriften zijn ideaal voor analisten die verhalen en context nodig hebben om met andere gebruikers te delen. Zakelijke gebruikers kunnen het gebruiken om snel op hoog niveau onderweg te ontdekken.

Bijvoorbeeld:

* **Input:** in CJA, stel een gesteunde visualisatie (met inbegrip van Lijn, Gebied, Grafiek van de Bar, Stroom, of Vallout) in werking, dan klik **[!UICONTROL Intelligent captions]**.

* **Output:** de mening auto-geproduceerde, natuurlijk-taaltitels die context en zeer belangrijke taken tonen. Vervolgens kunt u acties ondernemen met betrekking tot de gegenereerde gegevens, zoals controleren, kopiëren en delen met uw organisatie. [ zie hoe ](https://video.tv.adobe.com/v/3443144/?quality=12&learn=on#_blank&captions=dut)

[Meer informatie](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

**Content Analytics**

Content Analytics gebruikt AI en GenAI om automatisch metagegevens van elk element toe te wijzen, zoals onderwerpen, scènes, voorgrondkleuren, enzovoort. Een kenmerk is een door AI toegewezen metagegevenstag waarmee wordt beschreven wat zich in een element of ervaring bevindt.

Voorgrond `color: red` is bijvoorbeeld een automatisch toegewezen kenmerk. Met behulp van de visualisaties kunt u bepalen welke kenmerken van uw elementen het meest bijdragen aan de conversie. [Meer informatie](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/content-analytics/report/report#template)

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP gebruikt [!UICONTROL AI Assistant] om u te helpen met productkennis van Experience League. Het biedt ook operationele inzichten (in bèta). [!UICONTROL AI Assistant] vraagt naar een klantspecifieke gegevensopslag met operationele inzichten die gecentraliseerde operationele gegevens bevat, die in uw AEP-sandbox zijn gepartitioneerd. Het systeem trekt meta-gegevens slechts van Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s, en Bronnen, en heeft geen toegang tot gegevens binnen de zandbak.

Als u bijvoorbeeld een query uitvoert naar een publiek, heeft [!UICONTROL AI Assistant] toegang tot de naam van het publiek en andere bijbehorende metagegevens, maar heeft  geen toegang tot de profielen in dat publiek.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/home)

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Marketo] {#marketo}

In Marketo is generatieve AI beschikbaar in Interactieve Webinars en Dynamic Chat.

**Interactieve Webinars**

Produceer automatisch hoofdstukken en samenvattingen voor uw geregistreerde webinars, die hen toegankelijker en gemakkelijker maken om voor uw publiek te navigeren. Functies:

* Automatisch hoofdstuk genereren
* Door AI gegenereerde tekstsamenvatting
* Bewerkbare inhoud - gegenereerde hoofdstukken en samenvattingen wijzigen
* Eenvoudige integratie - Voeg hoofdstukken en samenvattingen toe aan uw bestemmingspagina&#39;s door de HTML-code naar de webpagina-editor van uw keuze te kopiëren

[Meer informatie](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai)

**Dynamic Chat**

Met de generatieve AI-functies in Adobe Dynamic Chat kunt u de productiviteit van uw verkoopagenten optimaliseren, inzicht krijgen in de intentie van uw websitebezoeker en op een veilige manier op bezoekersvragen reageren. U kunt de vragen, de antwoorden, en de gesprekssamenvatting vooraf goedkeuren. Dynamic Chat bevat zowel een gratis versie als een premiumversie.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Workfront] {#workfront}

[!UICONTROL AI Assistant] in [!DNL Workfront] helpt u bij het uitvoeren van uw werk door informatie en suggesties in de app aan te bieden. U kunt:

* Hiermee krijgt u samenvattingen van sommige objecten, zodat u de intentie of details van het object op een hoog niveau kunt bekijken.
* Stel vragen en laat [!UICONTROL AI Assistant] antwoorden zoeken op Experience League.
* Krijg geproduceerde formules op uw herinneringen worden gebaseerd die. U kunt fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden ook oplossen.
* Zoek projecten, taken en problemen.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## Aanvullende bronnen

* [ Verantwoordelijke AI Middelen op het Centrum van het Vertrouwen ](https://www.adobe.com/trust/responsible-ai.html) <!-- * [Customer AI Propensity Scoring Model Card](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/model-cards/ai-model-cards/customer-ai) -->

**Disclaimer:** de informatie op deze pagina is voor algemene informatiedoeleinden slechts. Hoewel er inspanningen worden geleverd om ervoor te zorgen dat de informatie accuraat en actueel blijft, kunnen software en generatieve AI-functies vaak veranderen. Daarom rechtvaardigen we niet te allen tijde de volledigheid, nauwkeurigheid of betrouwbaarheid van de informatie. Controleer alle belangrijke details voordat u beslissingen neemt op basis van deze inhoud.

