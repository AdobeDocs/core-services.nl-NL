---
title: AI in Experience Cloud-toepassingen
description: Leer over generatieve AI en hoe de toepassingen van Experience Cloud genAI en  [!DNL AI Assistant] gebruiken.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: d84fcf64b7019f0146340a423e8e20a932cd7874
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 2%

---

# AI in Experience Cloud-producten

Deze pagina helpt u te leren welke producten generatieve AI [!DNL AI Assistant] ondersteunen en of Adobe Firefly compatibel is. U vindt ook koppelingen naar productspecifieke Help-bronnen over het gebruik van AI in Experience Cloud.

**Ongeveer Generatieve AI**

Generatieve AI is een soort kunstmatige intelligentie die meer doet dan alleen vragen beantwoorden. Het kan __ inhoud tot stand brengen en _een reactie_ aan uw vragen of verklaringen produceren (die als _herinneringen_ worden bekend).

* **creeer:** de capaciteit om inhoud (tekst, beelden, muziek, of video&#39;s) van kras te produceren, die op zijn opleiding en inputherinneringen wordt gebaseerd. Dit vermogen is het _generatieve_ aspect van generatieve AI.

* **produceer een reactie:** AI verstrekt een antwoord of een reactie op een herinnering, typisch trekkend op zijn beschikbare gegevens en kennisbewaarplaatsen.

**wat is [!DNL AI Assistant]?**

[!DNL AI Assistant] is een conversatiegereedschap dat wordt ondersteund in Experience Platform en verwante toepassingen. Gebruik het om _productkennis_ snel te bereiken en, in gesteunde toepassingen, _operationele inzichten_ bijna onmiddellijk te bereiken.

* **Kennis van het Product:** de kennis van het Product verwijst naar concepten en onderwerpen die in de documentatie van Experience League worden gebaseerd. De antwoorden van Experience League zijn controleerbaar en worden met links genoemd. Leer over de types van [ op doelstelling-gebaseerde herinneringen ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) om het meeste uit [!DNL AI Assistant] te krijgen.

* **Operationele Inzichten:** de Operationele inzichten verwijzen naar antwoordenAI Medewerker produceert over uw voorwerpen van meta- gegevens (attributen, publiek, dataflows, datasets, bestemmingen, reizen, schema&#39;s, en bronnen), met inbegrip van tellingen, raadplegingen, en lijneffect. Met AI Assistant kunt u operationele inzichten in seconden in plaats van uren detecteren.

[Meer informatie](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company.
 -->

## Beschikbaarheid van AI in Experience Cloud-producten

Meer informatie over ondersteuning voor generatieve AI of [!DNL AI Assistant] in Experience Cloud-producten. Ondersteuning voor Adobe Firefly wordt ook aangegeven.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager Sites]](#aem-sites)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] Beheerde cloudservices](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Customer Journey Analytics]](#cja-captions)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## Adobe GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] is een door AI aangedreven platform dat u de mogelijkheid biedt om marketinginhoud te genereren en te beheren die voldoet aan uw merkstandaarden en voldoet aan uw bedrijfsbeleid. Inhoud genereren voor e-mails, metagegevens, LinkedIn-advertenties, weergaveadvertenties en banners.

U kunt GenStudio for Performance Marketing ook trainen op uw merk met voorbeelden, beschrijvingen van klantenpersonen en producten, en merkrichtlijnen.

[Meer informatie](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)

Verenigbaarheid met Adobe Firefly: **ja**

## Adobe [!DNL Experience Manager Sites] {#aem-sites}

In AEM Sites kunt u _[!UICONTROL Generate Variations]_gebruiken. Deze functie gebruikt generatieve kunstmatige intelligentie om inhoudvariaties te creëren die op uw inputherinneringen worden gebaseerd. Prompts worden geleverd door Adobe of gemaakt en beheerd door u.

Na het creëren van variaties, kunt u de inhoud op uw website gebruiken en zijn succes meten gebruikend de [ eigenschap van de Experimentatie ](https://www.aem.live/docs/experimentation) in Edge Delivery Services. U kunt ook afbeeldingen genereren in Adobe Express met behulp van de generatieve AI-mogelijkheden van Firefly.

**Input en outputvoorbeelden**

Invoervelden zijn:

* Aantal te genereren variaties
* Publiek Source
* Doelgroep publiek
* Aanvullende context
* Door de klant gestuurde vragen

De output is geproduceerde inhoud of marktexemplaar.

[ leer meer over produceer Variaties ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

Verenigbaarheid met Adobe Firefly: **ja**

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO), kunt u [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) gebruiken om _productkennis_ en _operationele inzichten_ (bèta) te bereiken.

### Voorbeelden van het gebruik van AI Assistant in AJO

Hier volgt een voorbeeldinput voor productkennis:

* _Hoeveel levende activiteiten kan ik in één zandbak van Journey Optimizer hebben?_

  De uitvoer wordt gegenereerd vanuit Experience League en andere Adobe-gegevensopslagruimten.

Hier volgt een voorbeeldinput voor operationele inzichten:

* _hoeveel Reizen in de laatste zeven dagen zijn gecreeerd?_

  Voor output, vraagt de Medewerker van AI een klant-specifieke gegevensopslag. De gegevensopslag bevat gecentraliseerde, operationele gegevens over [!UICONTROL Journeys]. Deze functie is onduidelijk voor de klant en haalt alleen metagegevens van zakelijke objecten op. Er worden geen gegevens in uw sandbox geopend.

[Meer informatie](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

Verenigbaarheid met Adobe Firefly: **Nr**

### AI Assistant voor het genereren van inhoud (AJO Prime en Ultimate) {#ajo-prime}

In AJO _Prime_ en _Ultimate_, kunt u [ inhoudsgeneratie ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) voor inhoudsgeneratie gebruiken om pro-actieve suggesties van de inhoudsvariatie voor tekst en beelden te brengen.

Deze functie is beschikbaar voor e-mail, pushberichten, webpagina&#39;s, inhoud en SMS-kanalen. Deze biedt snel gebaseerde tekst en het genereren van afbeeldingen. Uitvoer van het genereren van inhoud in AJO Prime en Ultimate is gegarandeerd.

[Meer informatie](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Verenigbaarheid met Adobe Firefly: **ja**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B edition gebruikt [!DNL AI Assistant] om u te helpen met productkennis.

Voorbeeld-invoer:

* _hoe ik een e-mail in een rekeningsreis verzend?_

  De uitvoer van productkennis wordt vanuit Experience League opgehaald.

[Meer informatie](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Verenigbaarheid met Adobe Firefly: **Nr**

## [!DNL Campaign] Beheerde cloudservices {#campaign-cs}

Met Campagne Managed Cloud Services wordt [!DNL AI Assistant] gebruikt voor het genereren van inhoud. Met deze functie kunt u automatisch gepersonaliseerde, aantrekkelijke en effectieve inhoud genereren op basis van uw marketingdoelstelling, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, tinten en meer met een merknaam. U kunt het gebruiken over kanalen zoals e-mail, SMS, en duw.

**Nota:** de Output van inhoudsgeneratie in de Beheerde Diensten van de Wolk van de Campagne wordt bevestigd.

[Meer informatie](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Verenigbaarheid met Adobe Firefly: **ja**

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics gebruikt [!DNL AI Assistant] om u te helpen productkennis en -inzichten van Experience League te ontdekken.

Als u een nieuwe gebruiker bent, leert u snel de concepten van Customer Journey Analytics en neemt u uzelf op voor producten en functies. Bijvoorbeeld:

* _hoe ik een e-mail in een rekeningsreis verzend?_

Ervaren gebruikers krijgen geavanceerde gebruiksgevallen of leren strategieën om taken snel uit te voeren. U kunt concepten snel begrijpen, problemen oplossen, of naar informatie zoeken.

[Meer informatie](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

Verenigbaarheid met Adobe Firefly: **Nr**

## [!DNL Customer Journey Analytics] {#cja-captions}

U kunt _Intelligente Bijschriften_ in [!DNL Customer Journey Analytics] gebruiken om natuurlijk-taalinzichten voor de het vaakst gebruikte Workspace visualisaties te krijgen. Intelligente bijschriften zijn ideaal voor analisten die verhalen en context nodig hebben om met andere gebruikers te delen. Zakelijke gebruikers kunnen het gebruiken om snel op hoog niveau onderweg te ontdekken.

Bijvoorbeeld:

* **Input:** in CJA, stel een gesteunde visualisatie (met inbegrip van Lijn, Gebied, Grafiek van de Bar, Stroom, of Vallout) in werking, dan klik **[!UICONTROL Intelligent captions]**.

* **Output:** de mening auto-geproduceerde, natuurlijk-taaltitels die context en zeer belangrijke taken tonen. Vervolgens kunt u acties ondernemen met betrekking tot de gegenereerde gegevens, zoals controleren, kopiëren en delen met uw organisatie. [ zie hoe ](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[Meer informatie](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

Verenigbaarheid met Adobe Firefly: **Nr**

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP gebruikt [!DNL AI Assistant] om u te helpen met productkennis van Experience League. Het biedt ook operationele inzichten (in bèta). [!DNL AI Assistant] vraagt naar een klantspecifieke gegevensopslag met operationele inzichten die gecentraliseerde operationele gegevens bevat, die in uw AEP-sandbox zijn gepartitioneerd. Het systeem trekt meta-gegevens slechts van Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s, en Bronnen, en heeft geen toegang tot gegevens binnen de zandbak.

Als u bijvoorbeeld een query uitvoert naar een publiek, heeft [!DNL AI Assistant] toegang tot de naam van het publiek en andere bijbehorende metagegevens, maar heeft  geen toegang tot de profielen in dat publiek.

[Meer informatie](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)

Verenigbaarheid met Adobe Firefly: **Nr**

## [!DNL Marketo] {#marketo}

Met de generatieve AI-functies in Adobe Dynamic Chat kunt u de productiviteit van uw verkoopagenten optimaliseren, inzicht krijgen in de intentie van uw websitebezoeker en op een veilige manier op bezoekersvragen reageren. U kunt de vragen, de antwoorden, en de gesprekssamenvatting vooraf goedkeuren.

[Meer informatie](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Verenigbaarheid met Adobe Firefly: **Nr**

## [!DNL Workfront] {#workfront}

[!DNL AI Assistant] in [!DNL Workfront] helpt u bij het uitvoeren van uw werk door informatie en suggesties in de app aan te bieden. U kunt:

* Hiermee krijgt u samenvattingen van sommige objecten, zodat u de intentie of details van het object op een hoog niveau kunt bekijken.
* Stel vragen en laat [!DNL AI Assistant] antwoorden zoeken op Experience League.
* Krijg geproduceerde formules op uw herinneringen worden gebaseerd die. U kunt fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden ook oplossen.
* Zoek projecten, taken en problemen.

[Meer informatie](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Verenigbaarheid met Adobe Firefly: **Nr**
