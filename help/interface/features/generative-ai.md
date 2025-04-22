---
title: AI in Experience Cloud-toepassingen
description: Leer meer over generatieve AI en hoe Experience Cloud-toepassingen genAI en AI Assistant gebruiken.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: aad561869cdfa7ddbc66b296d0a46c8f49f83d94
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 2%

---

# AI in Experience Cloud-toepassingen

Op deze pagina krijgt u meer inzicht in generatieve AI en hoe u deze kunt gebruiken in Experience Cloud-toepassingen. Leer welke productfuncties generatieve AI, AI Assistant gebruiken en of Adobe Firefly wordt ondersteund.

## Over generatieve AI en AI Assistant

Generatieve AI is een soort kunstmatige intelligentie die meer doet dan alleen vragen beantwoorden. Het _leidt tot_ inhoud en _antwoordt_ aan uw _herinneringen_ (vragen en verklaringen).

* **creeer:** verwijst naar de capaciteit van AI om nieuwe inhoud (tekst, beelden, muziek, of video&#39;s) van kras te produceren, die op zijn opleiding en inputherinneringen wordt gebaseerd. Dit vermogen is het _generatieve_ aspect van generatieve AI.

* **antwoordt:** verwijst naar AI die een antwoord of een reactie op een specifieke herinnering verstrekken, typisch het trekken van op zijn kennis of het redeneren mogelijkheden.

Als je nog geen ervaring hebt met Experience Cloud, kun je snel met generatieve AI productkennis opdoen. Als ervaren gebruiker, kunt u operationele inzichten in seconden eerder dan uren ontdekken.

### AI-assistent

[ AI Medewerker ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) is een gesprekshulpmiddel dat in Experience Platform en verwante toepassingen wordt gesteund. Gebruik het om uw werkschema&#39;s te versnellen, uw productkennis te verbeteren, problemen op te lossen, of door informatie te zoeken. In bepaalde toepassingen, laat AI Medewerker u operationele inzichten onmiddellijk ontdekken.

De antwoorden van Experience League op productkennis zijn verifieerbaar en worden met koppelingen genoemd. Leer over de types van [ op doelstelling-gebaseerde herinneringen ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) om de meesten uit AI Medewerker te krijgen.

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## Toepassingen met functies die ondersteuning bieden voor AI

* [GenStudio for Performance Marketing](#gspm)
* [Variaties genereren in AEM Sites (Cloud Service)](#aem-sites)
* [AI Assistant in Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime en Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B-editie](#ajo-b2b)
* [AI Assistant in Journey Optimizer Prime en Ultimate](#ajo-prime-ultimate)
* [AI Assistant in Journey Optimizer B2B edition](#ajo-b2b)
* [AI Assistant in Campagne Managed Cloud Services](#campaign-cs)
* [AI Assistant in Customer Journey Analytics](#cja)
* [Intelligente bijschriften in Customer Journey Analytics](#cja-captions)
* [AI Assistant in Real-Time CDP](#rtcdp)
* [Dynamic Chat in Marketo](#marketo)
* [AI Assistant in Workfront](#workfront)

### GenStudio for Performance Marketing {#gspm}

[ GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is een generatief AI-gedreven platform met mogelijkheden die kunnen transformeren hoe de marketing inhoud wordt gecreeerd, herzien, gedeeld en geanalyseerd.

Op [ creeer ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview) huis, kunt u high-Performance, ervaringen on-brand tot stand brengen. Inhoud genereren voor:

* E-mails
* Metaadvertenties
* LinkedIn-advertenties
* Advertenties weergeven
* Banners

U kunt GenStudio for Performance Marketing ook trainen op uw merk met voorbeelden, beschrijvingen van klantenpersonen en producten, en merkrichtlijnen. [Meer informatie...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Compatibel met Adobe Firefly:** Gepland

### Variaties genereren in Experience Manager Sites {#aem-sites}

[ produceer Variaties ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations) in AEM Sites gebruik generatieve AI om inhoudvariaties tot stand te brengen die op herinneringen worden gebaseerd. Deze herinneringen worden of verstrekt door [ Adobe ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) of gecreeerd en door [ gebruikers ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt) geleid.

Nadat u variaties hebt gemaakt, kunt u de inhoud op uw website gebruiken en het succes ervan meten met de functie Experimenteren in Edge Delivery Services.

### Invoer- en uitvoervelden

Invoervelden zijn:

* Aantal te genereren variaties
* Publiek Source
* Doelgroep publiek
* Aanvullende context
* Door de klant gestuurde vragen

De output is geproduceerde inhoud of marktexemplaar.

U kunt ook afbeeldingen genereren in Adobe Express met behulp van de generatieve AI-mogelijkheden van Firefly. [Meer informatie...](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)

**Compatibel met Adobe Firefly:** ja

## AI Assistant in Journey Optimizer {#journey-optimizer}

In Journey Optimizer kunt u met AI Assistant productkennis en operationele inzichten opdoen.

**de kennis van het Product:** AI Medewerker vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. De output is klantgewaarmerkt.

Voorbeeld:

* _Hoeveel levende activiteiten kan ik in één zandbak van Adobe Journey Optimizer hebben?_

**Operationele Inzichten (Beta)** - AI Medewerker vraagt een klant-specifieke operationele opslag van inzichten die gecentraliseerde operationele gegevens over Reizen bevat, die door de zandbak van de klant wordt verdeeld. Deze functie haalt alleen metagegevens van zakelijke objecten en heeft geen toegang tot gegevens in de sandbox.

Voorbeeld:

* _hoeveel Reizen in de laatste zeven dagen zijn gecreeerd?_

De uitvoer van de operationele inzichten is afhankelijk van metagegevens die uit de zakelijke objecten van de klant zijn gehaald. Deze output is klantgewaarmerkt.

_de Reizen_ is het enige voorwerp beschikbaar voor AI Medewerker in Journey Optimizer, en de meta-gegevens worden getrokken uit de huidige zandbak. [ leer meer... ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Compatibel met Adobe Firefly:** Nr

## AI Assistant in Journey Optimizer Prime en Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime en Ultimate gebruiken [ AI Medewerker voor de Versneller van de Inhoud ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) om pro-actieve suggesties van de inhoudsvariatie voor tekst en beelden te brengen.

Deze eigenschap is beschikbaar voor [ e-mail ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [ duw berichten ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [ Web-pagina ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [ inhoud ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation), en [ SMS ](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) kanalen. Deze biedt snel gebaseerde tekst en het genereren van afbeeldingen.

**Nota:** de Output van de Versneller van de Inhoud in AJO Prime en Ultimate wordt gecompenseerd.

**Compatibel met Adobe Firefly:** ja

## AI Assistant in Journey Optimizer B2B edition {#ajo-b2b}

Journey Optimizer B2B edition gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview) om u met productkennis te helpen, die op uw herinneringen van de productkennis wordt gebaseerd.

**de kennis van het Product** - vraagt de gegevensopslag van Adobe (zoals het productdocumentatie van Experience League) voor product insight. Deze output is klantgewaarmerkt.

* **Input:** hoe verzend ik een e-mail in een rekeningsreis?

* **Output:** de impulsen van de Kennis van het Product van Experience League (openbare documentatie). [Meer informatie...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/question-guidance)

**Compatibel met Adobe Firefly:** Nr

## AI Assistant in Campagne Managed Cloud Services {#campaign-cs}

De campagne Beheerde Diensten van de Wolk gebruikt [ AI Medewerker voor de Versneller van de Inhoud ](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs). Met deze functie kunt u automatisch gepersonaliseerde, aantrekkelijke en effectieve inhoud genereren op basis van uw marketingdoelstelling, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, tinten en meer met een merknaam. U kunt het over kanalen als [ e-mail ](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) gebruiken, [ SMS ](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms), en [ duw ](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push).

**Nota:** de Output van de Versneller van de Inhoud in de Campagne Beheerde Diensten van de Wolk wordt bevestigd.

**Compatibel met Adobe Firefly:** ja

## AI Assistant in Customer Journey Analytics {#cja}

Customer Journey Analytics gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) om u te helpen productkennis en inzichten van Experience League ontdekken.

**herinnering van het Voorbeeld:** hoe ik berekende metrisch bouwt?

De nieuwe gebruikers kunnen het gebruiken om de concepten van Customer Journey Analytics te leren en zich aan boord te nemen aan producten en eigenschappen die u niet kent.

Ervaren gebruikers kunnen de Medewerker van AI gebruiken om geavanceerdere gebruiksgevallen of uiteinden en trucs voor te stellen en taken in een snel tempo uit te voeren. Begrijp concepten, los problemen op, of onderzoek naar informatie. [Meer informatie...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge)

**Compatibel met Adobe Firefly:** Nr

## Intelligente bijschriften in Customer Journey Analytics {#cja-captions}

[ Intelligente Bijschriften ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) in Customer Journey Analytics verstrekken natuurlijk-taalinzichten voor de het vaakst gebruikte beelden van Workspace.

**Compatibel met Adobe Firefly:** Nr

## AI Assistant in Real-Time CDP {#rtcdp}

Real-Time CDP gebruikt [ AI Medewerker ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) om u te helpen productkennis en inzichten van Experience League ontdekken. [ krijgt uiteinden ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions) op het stellen van vragen.

Het biedt ook operationele inzichten (in bèta). De Medewerker van AI vraagt een klant-specifieke operationele opslag van inzichten die gecentraliseerde operationele gegevens bevat, die door de zandbak van AEP van de klant worden verdeeld. Het trekt meta-gegevens slechts van Attributen, Soorten publiek, Dataflows, Datasets, Doelen, Schema&#39;s, en Bronnen, en heeft geen toegang tot gegevens binnen de zandbak.

Voor een query over een publiek heeft [!DNL AI Assistant] bijvoorbeeld toegang tot de naam van het publiek en andere bijbehorende metagegevens, maar heeft  geen toegang tot de profielen in dat publiek.

Bijvoorbeeld:

* Invoer: _hoeveel datasets heb ik?_

* Reactie: De uitvoer van operationele inzichten is afhankelijk van de metagegevens die uit de zakelijke objecten van de klant zijn opgehaald (kenmerken, soorten publiek, gegevensstromen, gegevenssets, doelen, schema&#39;s en bronnen) en bevat een koppeling naar een specifieke UI-pagina met opgevraagde gegevens.

Voor meer voorbeelden, zie de _Kennis van het Product_ en _Operationele Inzichten_ inputlijsten in [ AI Medewerker in Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)

**Compatibel met Firefly:** Nr

## Dynamic Chat in Marketo {#marketo}

Met de generatieve AI-functies in Adobe Dynamic Chat kunt u de productiviteit van uw verkoopagenten optimaliseren, inzicht krijgen in de intentie van uw websitebezoeker en op een veilige manier op bezoekersvragen reageren. U kunt de vragen, de antwoorden, en de gesprekssamenvatting vooraf goedkeuren. [Meer informatie...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

**Compatibel met Firefly:** Nr

## AI Assistant in Workfront {#workfront}

Met AI Assistant in Workfront kunt u uw werk uitvoeren door informatie en suggesties in de app te bieden. U kunt:

* Hiermee krijgt u samenvattingen van sommige objecten, zodat u de intentie of details van het object op een hoog niveau kunt bekijken.
* Stel vragen en laat [!DNL AI Assistant] antwoorden zoeken op Experience League.
* Krijg geproduceerde formules op uw herinneringen worden gebaseerd die. U kunt fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden ook oplossen.
* Zoek projecten, taken en problemen.

[Meer informatie...](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

**Compatibel met Firefly:** Nr
