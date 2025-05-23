---
title: AI in Experience Cloud-toepassingen
description: Leer over generatieve AI (GenAI) en hoe de toepassingen van Experience Cloud gebruiken GenAI en  [!DNL AI Assistant].
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 73ae5b86dd0309974b607e93e8cf93dcdfcc40c7
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 2%

---

# Generatieve AI in Experience Cloud-producten

Op deze pagina kunt u zien welke producten generatieve AI (GenAI), [!DNL AI Assistant] ondersteunen en of Adobe Firefly compatibel is. U vindt ook koppelingen naar informatie over verschillende manieren waarop u AI kunt gebruiken in Experience Cloud-toepassingen.

**Ongeveer Generatieve AI**

Generatieve AI is een type AI-bestand dat originele inhoud kan maken, zoals tekst, afbeeldingen, video, audio of softwarecode als reactie op een vraag of verzoek van een gebruiker.

* **creeer:** de capaciteit om inhoud (tekst, beelden, muziek, of video&#39;s) van kras te produceren, die op zijn opleiding en inputherinneringen wordt gebaseerd. Dit vermogen is het _generatieve_ aspect van generatieve AI.

* **produceer een reactie:** AI verstrekt een antwoord of een reactie op een herinnering, typisch trekkend op zijn beschikbare gegevens en kennisbewaarplaatsen.

**wat is [!DNL AI Assistant]?**

[!DNL AI Assistant] is een conversatiegereedschap dat wordt ondersteund in Experience Platform en verwante toepassingen. Gebruik het om _productkennis_ en, in gesteunde producten snel te bereiken, _operationele inzichten_ bijna onmiddellijk.

* **de kennis van het Product:** de kennis van het Product verwijst naar concepten en onderwerpen die in de documentatie van Experience League worden gegrond. Leer hoe te om efficiënte, [ op doelstelling-gebaseerde herinneringen ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/home) tot stand te brengen om het meeste uit [!DNL AI Assistant] te krijgen. Alle antwoorden van Experience League zijn controleerbaar en worden met links genoemd.

* **Operationele inzichten:** [ Operationele inzichten ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/questions#objects-questions) verwijzen naar geproduceerde reacties over uw meta-gegevensvoorwerpen (attributen, publiek, dataflows, datasets, etc.). Met AI Assistant kunt u in seconden bereiken wat anders uren of dagen kan duren.

[ Leer over Medewerker AI ](https://experienceleague.adobe.com/nl/docs/experience-platform/ai-assistant/landing)

<!--## Adobe Marketing Agent for Microsoft 365 Copilot 

The Adobe Marketing Agent for Microsoft 365 Copilot is a generative AI-powered assistant designed to enhance marketing workflows by integrating Adobe's marketing capabilities directly into Microsoft 365 applications such as Word, PowerPoint, Teams, and Outlook. This collaboration between Adobe and Microsoft aims to streamline marketing processes, allowing marketers to access insights and tools within their existing work environments.
Adobe for Business

Key features and capabilities:

**Audience Refinement:** Marketers can use natural language prompts within Microsoft 365 to access data and insights from Adobe Experience Platform, enabling quick audience analysis and segmentation for personalized campaigns. 

**Insight Discovery:** The agent can retrieve meaningful insights from Adobe Customer Journey Analytics, facilitating the creation of campaign performance reports directly within Microsoft apps, thus supporting informed decision-making. 

**Content Creation:** Through integration with Adobe Express, users can generate high-quality images and assets within Microsoft 365 applications, aiding in the development of presentations, documents, and social media content. 
Adobe Newsroom

**Workflow Optimization:** The agent can automate tasks in Adobe Workfront, manage content approvals, and provide real-time alerts in Microsoft Teams based on analytics data, enhancing operational efficiency. 

**Campaign Performance Monitoring:** Users can query the agent for campaign performance metrics, which can be visualized and incorporated into PowerPoint presentations for easy sharing and analysis. 
Adobe for Business

Currently in private preview, the Adobe Marketing Agent for Microsoft 365 Copilot is expected to be generally available later in 2025. This integration represents a significant step in unifying marketing tools and data, aiming to improve productivity and collaboration for marketing teams.
 -->

## beschikbaarheid van GenAI in Experience Cloud-producten

Leer hoe de volgende Experience Cloud-toepassingen generatieve AI of [!DNL AI Assistant] ondersteunen. Ondersteuning voor Adobe Firefly wordt ook aangegeven.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager]](#aem)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] Beheerde cloudservices](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## Adobe GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] is een door AI aangedreven platform dat u de mogelijkheid biedt om marketinginhoud te genereren en te beheren die voldoet aan uw merkstandaarden en voldoet aan uw bedrijfsbeleid. Inhoud genereren voor e-mails, metagegevens, LinkedIn-advertenties, weergaveadvertenties en banners.

U kunt GenStudio for Performance Marketing ook trainen op uw merk met voorbeelden, beschrijvingen van klantenpersonen en producten, en merkrichtlijnen.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/genstudio-for-performance-marketing/user-guide/home)

De verenigbaarheid van Adobe Firefly: **ja**

## Adobe [!DNL Experience Manager] {#aem}

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

[ leer meer over produceer Variaties ](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

### Experience Manager Assets

[!UICONTROL Content Hub] is beschikbaar als onderdeel van [!DNL Experience Manager Assets as a Cloud Service] voor het democratiseren van de toegang tot online-inhoud voor organisaties en hun zakelijke partners. Het richt zich op het distribueren van middelen voor activering op schaal en het creëren van varianten van on-brand-inhoud met het oog op verbeterde marketingflexibiliteit.

In Content Hub kunt u inhoud maken met Adobe Express (als u Adobe Express-rechten hebt). U kunt bestaande inhoud bewerken met eenvoudige gereedschappen, merkvariaties produceren met sjablonen en merkelementen en inhoud maken met de nieuwste GenAI-mogelijkheden van [!DNL Adobe Firefly] .

[Meer informatie](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview)

De verenigbaarheid van Adobe Firefly: **ja**

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO), kunt u [ AI Medewerker ](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/get-started/ai-assistant) gebruiken om _productkennis_ en _operationele inzichten_ (bèta) te bereiken.

### Voorbeelden van het gebruik van AI Assistant in AJO

Hier volgt een voorbeeldinput voor productkennis:

* _Hoeveel levende activiteiten kan ik in één zandbak van Journey Optimizer hebben?_

  De uitvoer wordt gegenereerd vanuit Experience League en andere Adobe-gegevensopslagruimten.

Hier volgt een voorbeeldinput voor operationele inzichten:

* _hoeveel Reizen in de laatste zeven dagen zijn gecreeerd?_

  Voor output, vraagt de Medewerker van AI een klant-specifieke gegevensopslag. De gegevensopslag bevat gecentraliseerde, operationele gegevens over [!UICONTROL Journeys]. Deze functie is onduidelijk voor de klant en haalt alleen metagegevens van zakelijke objecten op. Er worden geen gegevens in uw sandbox geopend.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/get-started/ai-assistant).

De verenigbaarheid van Adobe Firefly: **Nr**

### AI Assistant voor het genereren van inhoud (AJO Prime en Ultimate) {#ajo-prime}

In AJO _Prime_ en _Ultimate_, kunt u [ inhoudsgeneratie ](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) voor inhoudsgeneratie gebruiken om pro-actieve suggesties van de inhoudsvariatie voor tekst en beelden te brengen.

Deze functie is beschikbaar voor e-mail, pushberichten, webpagina&#39;s, inhoud en SMS-kanalen. Deze biedt snel gebaseerde tekst en het genereren van afbeeldingen. Uitvoer van het genereren van inhoud in AJO Prime en Ultimate is gegarandeerd.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

De verenigbaarheid van Adobe Firefly: **ja**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B edition gebruikt [!DNL AI Assistant] om u te helpen met productkennis.

Voorbeeld-invoer:

* _hoe ik een e-mail in een rekeningsreis verzend?_

  De uitvoer van productkennis wordt vanuit Experience League opgehaald.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Campaign] Beheerde cloudservices {#campaign-cs}

Met Campagne Managed Cloud Services wordt [!DNL AI Assistant] gebruikt voor het genereren van inhoud. Met deze functie kunt u automatisch gepersonaliseerde, aantrekkelijke en effectieve inhoud genereren op basis van uw marketingdoelstelling, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, tinten en meer met een merknaam. U kunt het gebruiken over kanalen zoals e-mail, SMS, en duw.

**Nota:** de Output van inhoudsgeneratie in de Beheerde Diensten van de Wolk van de Campagne wordt bevestigd.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/campaign-web/v8/content/ai-assistant/generative-gs)

De verenigbaarheid van Adobe Firefly: **ja**

## [!DNL Customer Journey Analytics] {#cja}

Met Customer Journey Analytics kunt u op de volgende manieren generatieve AI gebruiken:

* [!DNL AI Assistant] voor productkennis en -inzichten
* [!UICONTROL Intelligent Captions] in Workspace-visualisaties
* AI en GenAI om metagegevens van elk element automatisch toe te wijzen in [!DNL Content Analytics]

**AI Medewerker**

Kennis en inzichten van producten van Experience League ontdekken. Als u een nieuwe gebruiker bent, leert u snel de concepten van Customer Journey Analytics en neemt u uzelf op voor producten en functies. Bijvoorbeeld:

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

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP gebruikt [!DNL AI Assistant] om u te helpen met productkennis van Experience League. Het biedt ook operationele inzichten (in bèta). [!DNL AI Assistant] vraagt naar een klantspecifieke gegevensopslag met operationele inzichten die gecentraliseerde operationele gegevens bevat, die in uw AEP-sandbox zijn gepartitioneerd. Het systeem trekt meta-gegevens slechts van Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s, en Bronnen, en heeft geen toegang tot gegevens binnen de zandbak.

Als u bijvoorbeeld een query uitvoert naar een publiek, heeft [!DNL AI Assistant] toegang tot de naam van het publiek en andere bijbehorende metagegevens, maar heeft  geen toegang tot de profielen in dat publiek.

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

Met de generatieve AI-functies in Adobe Dynamic Chat kunt u de productiviteit van uw verkoopagenten optimaliseren, inzicht krijgen in de intentie van uw websitebezoeker en op een veilige manier op bezoekersvragen reageren. U kunt de vragen, de antwoorden, en de gesprekssamenvatting vooraf goedkeuren.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## [!DNL Workfront] {#workfront}

[!DNL AI Assistant] in [!DNL Workfront] helpt u bij het uitvoeren van uw werk door informatie en suggesties in de app aan te bieden. U kunt:

* Hiermee krijgt u samenvattingen van sommige objecten, zodat u de intentie of details van het object op een hoog niveau kunt bekijken.
* Stel vragen en laat [!DNL AI Assistant] antwoorden zoeken op Experience League.
* Krijg geproduceerde formules op uw herinneringen worden gebaseerd die. U kunt fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden ook oplossen.
* Zoek projecten, taken en problemen.

[Meer informatie](https://experienceleague.adobe.com/nl/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

De verenigbaarheid van Adobe Firefly: **Nr**

## Aanvullende bronnen

* [ Verantwoordelijke AI Middelen op het Centrum van het Vertrouwen ](https://www.adobe.com/trust/responsible-ai.html)
