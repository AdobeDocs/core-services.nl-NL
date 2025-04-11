---
title: AI in Experience Cloud-toepassingen
description: Leer hoe Experience Cloud-toepassingen generatieve AI en AI Assistant gebruiken.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
hide: false
hidefromtoc: true
index: n
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 4d784762d7d533b672e0cfa6944a3f26ebca0eaa
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 3%

---

# AI in Experience Cloud-toepassingen

Deze pagina helpt u te begrijpen hoe Experience Cloud-toepassingen generatieve AI gebruiken en waar u de toepassingsspecifieke informatie kunt vinden. Leer meer over de klassen vragen, vragen, en input en outputmodellen.

## Over generatieve AI en AI Assistant

Generatieve AI is een type van kunstmatige intelligentie die __ nieuwe inhoud kan creëren en __ aan uw verklaringen en vragen (herinneringen) antwoorden:

* **creeer:** verwijst naar de capaciteit van AI om nieuwe inhoud (tekst, beelden, muziek, of video&#39;s) van kras te produceren, die op zijn opleiding en inputherinneringen wordt gebaseerd. Dit vermogen is het _generatieve_ aspect van generatieve AI.

* **antwoordt:** verwijst naar AI die een antwoord of een reactie op een specifieke vraag, een verklaring, of een herinnering verstrekt, typisch het trekken van op zijn kennis of het redeneren mogelijkheden.

Bepaalde Experience Cloud-toepassingen maken gebruik van generatieve AI, waardoor nieuwe gebruikers snel productkennis kunnen opdoen en ervaren gebruikers in seconden in plaats van uren operationele inzichten ontdekken.

### AI-assistent

[ AI Medewerker ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) is een gesprekshulpmiddel dat in Experience Platform en verwante toepassingen wordt gesteund. Gebruik het om uw werkschema&#39;s te versnellen, uw productkennis te verbeteren, problemen op te lossen, of door informatie te zoeken. Met AI Assistant kunt u in seconden in plaats van uren operationele inzichten ontdekken.

Alle antwoorden op productkennis zijn verifieerbaar en worden aangehaald met koppelingen naar productdocumentatie in Experience League. [ leer over AI Medewerker ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) en de types van op doelstelling-gebaseerde herinneringen om het meeste uit AI Medewerker te krijgen.

## Experience Cloud-toepassingen die gebruikmaken van AI

>[!TIP]
>
>Subhead-versie (alleen een begin)...


* [Adobe GenStudio for Performance Marketing](#gspm)
* [Adobe Experience Manager Sites (Cloud Service)](#aem-sites)
* [Adobe Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime en Ultimate](#ajo-prime-ultimate)

### GenStudio for Performance Marketing {#gspm}

[ GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is een generatief AI-gedreven platform. De levenscyclus van het maken van inhoud wordt hierdoor beïnvloed door generatieve AI-mogelijkheden die de manier transformeren waarop marketinginhoud wordt gemaakt, gecontroleerd, gedeeld en geanalyseerd.

_GenStudio for Performance Marketing creeert_ hefboomwerkingen de macht van Adobe GenAI om marktleiders en verdeelde teams in staat te stellen om krachtige, onmerkervaringen tot stand te brengen. Inhoud genereren voor:

* E-mails
* Metaadvertenties
* LinkedIn-advertenties
* Advertenties weergeven
* Banners

U kunt GenStudio for Performance Marketing trainen op uw merk met voorbeelden, beschrijvingen van klantenpersonen en producten, en merkrichtlijnen. [ leer meer.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Verenigbaarheid met Adobe Firefly:** Gepland

### Experience Manager Sites {#aem-sites}

AEM Sites gebruikt [ produceert Variaties ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). Bij Variaties genereren wordt gebruikgemaakt van generatieve AI om inhoudvariaties te maken op basis van aanwijzingen. Deze prompts worden geleverd door [Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) of gemaakt en beheerd door [gebruikers](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Nadat u variaties hebt gemaakt, kunt u de inhoud van uw website gebruiken en het succes ervan meten met de functie Experimenteren van Edge Delivery Services.

**Input:** de gebieden van de Input omvatten:

* Aantal te genereren variaties
* Publiek Source
* Doelgroep
* Aanvullende context
* Klantgestuurde prompts

**Output:** Gegenereerde inhoud / Marktkopie. Je hebt ook de mogelijkheid om afbeeldingen te genereren in Adobe Express met behulp van de generatieve AI-mogelijkheden van Firefly.

Zie [Afbeelding](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image) genereren.

**Verenigbaarheid met Adobe Firefly:** ja

## Journey Optimizer {#journey-optimizer}

Journey Optimizer gebruikt [ Medewerker AI ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) met twee klassen van vragen:

**de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt. Voorbeeld:

* Hoeveel levende activiteiten kan ik in één zandbak van Adobe Journey Optimizer hebben?

**Operationele Inzichten (Beta)** - vraagt een klant-specifieke operationele opslag van inzichten die gecentraliseerde operationele gegevens over Reizen bevat, die door de zandbak van de klant wordt verdeeld. Hiermee worden metagegevens alleen door zakelijke objecten opgehaald en worden geen gegevens in de sandbox geopend.

* Hoeveel reizen zijn er gemaakt in de afgelopen zeven dagen?

De uitvoer van de operationele inzichten is afhankelijk van metagegevens die uit de zakelijke objecten van de klant zijn gehaald.

De reizen is het enige voorwerp beschikbaar voor AI Medewerker in Journey Optimizer, en de meta-gegevens worden getrokken uit de huidige zandbak.

Zie [ Werk met de Medewerker AI ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) en [ Gereedheid van het Gebied ](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) voor meer.

**Compatibiliteit met Adobe Firefly:** Nee

## Journey Optimizer Prime en Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime en Ultimate gebruiken [AI Assistant voor Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) om proactieve suggesties voor inhoudsvariatie voor tekst en afbeeldingen te bieden.

Deze functie is beschikbaar voor e-mail-, push-, web- en sms-kanalen. Het biedt prompt-based tekst- en afbeeldingsgeneratie.

**E-mail** - genereer een volledige e-mail, alleen tekst of alleen afbeelding. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email)

**het Bericht van de Duw** - produceer een volledig duw bericht, tekst slechts of beeld slechts. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push)

**SMS** - produceer volledige SMS, of slechts tekst. [Meer informatie](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms)

**Webpagina** - produceer Web-pagina beelden of Web-pagina tekst. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web)

**Inhoud** - produceer inhoud voor diverse overseinencampagnes. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)

**Nota:** de Output van de Versneller van de Inhoud in AJO Prime en Ultimate wordt gecompenseerd.

**Verenigbaarheid met Adobe Firefly:** ja

## Journey Optimizer B2B-editie {#ajo-b2b}

Gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) voor de herinneringen van de productkennis.

**de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt. | <ul><li>**Input:** hoe verzend ik een e-mail in een rekeningsreis?</li><li>**Output:** de impulsen van de Kennis van het Product van Experience League (openbare documentatie). [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | Nee   |

## Experience Cloud-toepassingen die gebruikmaken van AI

>[!TIP]
>
>Tabelversie...


Leer hoe Experience Cloud-toepassingen generatieve AI of AI Assistant gebruiken en of Adobe Firefly wordt ondersteund.

| Toepassing | Hoe generatieve AI wordt gebruikt | Voorbeelden | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [ GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is een generatief AI-gedreven platform. De levenscyclus van het maken van inhoud wordt hierdoor beïnvloed door generatieve AI-mogelijkheden die de manier transformeren waarop marketinginhoud wordt gemaakt, gecontroleerd, gedeeld en geanalyseerd.<br> u kunt GenStudio for Performance Marketing op uw merk trainen gebruikend voorbeelden, beschrijvingen van klantenpersona&#39;s en producten, en merkrichtlijnen. | _GenStudio for Performance Marketing creeert_ laat u inhoud voor e-mail, advertenties van Meta, LinkedIn advertenties, vertoningsadvertenties, en banners produceren. <br>**Inputs:** <ul><li>Gebruik sjablonen om het maken van inhoud te starten. </li><li>U kunt parameters als merken, producten en persoonlijke instellingen (richtlijnen) en inhoud (elementen) toevoegen om de gegenereerde ervaring vorm te geven. </li><li>Voer beschrijvende aanwijzingen in die de context of ervaring beschrijven die u wilt genereren. [Meer informatie...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> | Ja |
| Adobe Experience Manager Sites (Cloud Service) | AEM Sites gebruikt [ produceert Variaties ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br> produceer Variaties gebruik generatieve AI om inhoudvariaties tot stand te brengen die op herinneringen worden gebaseerd. Deze herinneringen worden verstrekt door Adobe of gecreeerd en door gebruikers geleid. | Nadat u variaties hebt gemaakt, kunt u de inhoud van uw website gebruiken en het succes ervan meten met de functie Experimenteren van Edge Delivery Services. <br>**Input:** de gebieden van de Input omvatten Aantal te produceren Variaties; het Doel van het publiek Source/van het Publiek; Extra Context, en klant-gedreven herinneringen. <ul><li>[ Adobe snel malplaatje ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[ Gebruiker produceerde herinnering ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** Gegenereerde inhoud / Marktkopie. Je hebt ook de mogelijkheid om afbeeldingen te genereren in Adobe Express met behulp van de generatieve AI-mogelijkheden van Firefly. Zie [Afbeelding](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image) genereren. | Ja |
| Adobe Journey Optimizer | Journey Optimizer gebruikt [ Medewerker AI ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) met twee klassen van vragen:<ul><li>**de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt. </li><li>**Operationele Inzichten (Beta)** - vraagt een klant-specifieke operationele opslag van inzichten die gecentraliseerde operationele gegevens over Reizen bevat, die door de zandbak van de klant wordt verdeeld. Hiermee worden metagegevens alleen door zakelijke objecten opgehaald en worden geen gegevens in de sandbox geopend.</li></ul> | <ul><li>**Invoer van de Kennis van het Product:** hoeveel levende activiteiten kan ik in één zandbak van Adobe Journey Optimizer hebben?</li><li>**Uitvoer van de Kennis van het Product:** trekt van de Kennis van het Product van Experience League (openbare documentatie). </li><li>**Operationele Input van Inzichten:** hoeveel Reizen in de laatste zeven dagen zijn gecreeerd? </li><li>**Operationele Uitvoer van Inzichten:** de operationele output van Inzichten hangt van meta-gegevens af die van de bedrijfsobjecten van de klant worden getrokken. De reizen is het enige voorwerp beschikbaar in AJO, en de meta-gegevens worden getrokken uit de huidige zandbak. </li></ul> Zie [ Werk met de Medewerker AI ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) en [ Gereedheid van het Gebied ](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | Nee |
| Journey Optimizer: _Prime_ en _Ultimate_ | [ AI Medewerker voor de Versneller van de Inhoud ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) brengt pro-actieve suggesties van de inhoudsvariatie voor tekst en beelden. Het is beschikbaar voor e-mail, duw, Web en de kanalen van SMS. Met deze nieuwe mogelijkheid kunnen tekst- en afbeeldingsgegevens op basis van prompts worden gegenereerd. | <ul><li> **E-mail** - genereer een volledige e-mail, alleen tekst of alleen afbeelding. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Pushmelding** - Genereer een volledige pushmelding, alleen tekst of alleen afbeelding. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Genereer een volledige sms, of alleen tekst. [Meer informatie](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Webpagina** - produceer Web-pagina beelden of Web-pagina tekst. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Inhoud** - produceer inhoud voor diverse overseinencampagnes. [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Nota:** de Output van de Versneller van de Inhoud in AJO Prime en Ultimate wordt gecompenseerd. | Ja |
| Journey Optimizer B2B-editie | Gebruikt [ Medewerker AI ](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) met één klasse van vragen: <br> **de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt. | <ul><li>**Input:** hoe verzend ik een e-mail in een rekeningsreis?</li><li>**Output:** de impulsen van de Kennis van het Product van Experience League (openbare documentatie). [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul> | Nee |
| Campagne Managed Cloud Services | [ AI Medewerker voor de Versneller van de Inhoud ](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-produceert gepersonaliseerde, het in dienst nemen, en efficiënte inhoud die op het marketing doel met inhoud wordt gebaseerd die voor merk geschetste stijlen, lay-outs, toon, en meer over kanalen zoals E-mail, SMS, Duw wordt geoptimaliseerd. | <ul><li> **E-mail** - produceer een volledige e-mail, tekst slechts of beeld slechts. [Meer informatie](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - produceer volledige SMS of slechts tekst. [Meer informatie...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **duw** - creeer het dwingen overseinen en produceer inhoud. [Meer informatie...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Nota:** de Output van de Versneller van de Inhoud in de Campagne Beheerde Diensten van de Wolk wordt bevestigd. | Ja |
| Customer Journey Analytics | CJA gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) om u te helpen productkennis en inzichten van Experience League ontdekken. <br> Bijvoorbeeld, kunnen de nieuwe gebruikers het gebruiken om de concepten van Customer Journey Analytics en aan boord van zich aan producten en eigenschappen te leren die u met onbekend bent. <br> ervaren gebruikers kunnen de Medewerker van AI gebruiken om geavanceerdere gebruiksgevallen of uiteinden en trucs voor te stellen en taken bij een snel tempo uit te voeren. Begrijp concepten, los problemen op, of onderzoek naar informatie. [Meer informatie...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Invoer van de Kennis van het Product:** hoe ik berekende metrisch bouwt? </li><li> **Uitvoer van de Kennis van het Product:** trekt van de Kennis van het Product van Experience League (openbare documentatie). </li></ul> | Nee |
| Customer Journey Analytics | [ Intelligente Bijschriften ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) verstrekt natuurlijk-taalinzichten voor lijnvisualisaties in Workspace visualisaties. | <ul><li>**Input:** de visualisaties van de Lijn. De titels worden auto-geproduceerd gebaseerd op dergelijke lijnvisualisaties wanneer u **Intelligente titels** klikt. </li><li> **Output:** Auto-geproduceerde natuurlijk-taaltitels.</li></ul> | Nee |
| Real-Time CDP | Gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) om u te helpen productkennis en inzichten van Experience League ontdekken. Het vraagt een gegevensbestand en vertaalt gegevens van het gegevensbestand in een mens-leesbaar antwoord. Twee klassen vragen: <br> **de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt. <br> **Operationele Inzichten (Beta)** - vraagt een klant-specifieke operationele opslag van inzichten die gecentraliseerde operationele gegevens bevat, die door de zandbak van AEP van de klant worden verdeeld. Hiermee worden alleen metagegevens opgehaald van Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s en Bronnen. De gegevens in de sandbox zijn niet toegankelijk. <br> bijvoorbeeld, voor een vraag over een publiek [!DNL AI Assistant] kan tot de naam van het publiek en andere bijbehorende meta-gegevens toegang hebben maar kan niet tot de profielen binnen dat publiek toegang hebben. | <ul><li>**Invoer van de Kennis van het Product:** Hoe wordt de profielrijkheid berekend? </li><li>**Uitvoer van de Kennis van het Product:** trekt van de Kennis van het Product van Experience League (openbare documentatie). </li><li> **Operationele Input van Inzichten:** hoeveel datasets heb ik? </li><li> **Operationele Uitvoer van Inzichten:** de operationele output van Inzichten hangt van meta-gegevens af die van de bedrijfsobjecten van de Klant (Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s, en Bronnen) worden getrokken, en omvat een verbinding aan specifieke pagina UI die gevraagde gegevens bevat. </li></ul>Voor voorbeelden, zie de _Kennis van het Product_ en _Operationele Inzichten_ inputlijsten in [ AI Medewerker in Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) | Nee |
| Marketo | [ Dynamic Chat ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) leidt tot AI-bijgewoonde gesprekken met aangepaste en vooraf goedgekeurde vragen en antwoorden, evenals gesprekssamenvatting | <ul><li> **produceer Vragen:** verstrek URLs waarvan de inhoud wordt gehaald en gebruikt om vragen/reacties te produceren. </li><li> **Samenvatting van de Gesprek:** produceert een samenvatting van een praatjegesprek. </li></ul> [Meer informatie...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library) | Nee |
| Workfront | [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helpt u uw werk verwezenlijken door in-app informatie en suggesties in een natuurlijk-taalgesprek aan te bieden. AI Assistant biedt de volgende functionaliteit: vat projecten/taken/problemen/documenten samen, geeft instructies of referentiegegevens die uit de Workfront-documentatie in Experience League zijn gehaald, genereert of verfijnt formules voor berekende aangepaste velden. | <ul><li>**vat de Input van het Project samen:** vat dit project samen </li><li> **Projectuitvoer samenvatten:** Geeft korte beschrijvingen van het doel en de status van het project, geeft voorbeelden van taken die zijn voltooid en die nog in behandeling zijn, en biedt enkele aanvullende details en notities.</li><li> **Formule-invoer genereren/verfijnen:** &quot;Herschrijf deze formule om de ongeldige expressiefout te verwijderen.&quot; </li><li> **Formule genereren/verfijnen Output:** Gegenereerde of verfijnde formule. </li></ul>**Opmerking:** Het kan even duren voordat de AI-assistent de herziene formule heeft gegenereerd, afhankelijk van de grootte en complexiteit van de formule. | Nee |
