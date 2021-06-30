---
description: Leer hoe u kenmerkregels gebruikt om een publiek te maken en een samengesteld publiek in Adobe Experience Cloud te definiëren.
keywords: kerndiensten
solution: Experience Cloud
title: 'Een doelgroep maken '
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Auditiebibliotheek
topic: Beheer
role: Administrator
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: 93f5eda7229990e3645b54efa2a172d7b57dcb9b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 2%

---

# Een doelgroep maken

Leer hoe te om attributenregels te gebruiken om een publiek tot stand te brengen en een samengesteld publiek in Experience Cloud te bepalen.

Dit artikel helpt u begrijpen hoe te:

* Een doelgroep maken
* Een regel maken
* Regels gebruiken om een samengesteld publiek te definiëren

De volgende afbeelding vertegenwoordigt twee regels in een samengesteld publiek.

![](assets/audience_sharing.png)

Elke cirkel vertegenwoordigt een regel die publiekslidmaatschap bepaalt. Bezoekers die als leden in beide publieksregels worden gekwalificeerd, overlappen elkaar om het samengestelde, gedefinieerde publiek te worden.

>[!NOTE]
>
>Het publiek wordt volledig gedefinieerd nadat de gegevensverzameling voor de opgegeven periode is voltooid.

In het volgende voorbeeld ziet u hoe u de regels voor een samengesteld publiek maakt. Dit publiek bestaat uit:

* De sectie Home &amp; Garden is afgeleid van paginagegevens of onbewerkte analysegegevens.
* Chrome- en Safari-gebruikers zijn afgeleid van een [!DNL Adobe Analytics]-segment [gepubliceerd](audience-library.md#task_32FEEFE0B32E4E388CD4D892D727282A) naar [!DNL Experience Cloud].

   ![](assets/audience_create.png)

**Een publiek maken**

1. Selecteer **[!UICONTROL People]** > **[!UICONTROL Audience Library]onder [!DNL Experience Cloud].**[!DNL Experience Platform]
1. Selecteer **[!UICONTROL New]** op de pagina [!UICONTROL Audiences]. ![](assets/add_icon_small.png)

   ![Stap Resultaat](assets/audience_create_new.png)

1. Geef op de pagina [!UICONTROL Create New Audience] een titel en een beschrijving op.
1. Selecteer onder [!UICONTROL Rules] een kenmerkbron:

   * **[!UICONTROL Real-Time Analytics Data:]** (of Raw-gegevens) Dit zijn kenmerkgegevens die zijn afgeleid van Real-Time Analytics-afbeeldingsaanvragen en die gegevens bevatten zoals eVars en gebeurtenissen. U moet een rapportreeks selecteren wanneer het gebruiken van deze attributenbron, en de dimensie of de gebeurtenis bepalen om te omvatten. Deze selectie van de rapportreeks verstrekt de veranderlijke structuur die door de rapportreeks wordt gebruikt.
   >[!NOTE]
   >
   >Als gevolg van caching, vereisen de geschrapte rapportreeksen in Analytics 12 uur alvorens de schrapping in de Experience Cloud wordt getoond.

   * **[!UICONTROL Experience Cloud:]** Kenmerkgegevens die zijn afgeleid van de  [!DNL Experience Cloud] bronnen. Dit kunnen bijvoorbeeld gegevens zijn van publiekssegmenten die u maakt in [!DNL Analytics] of gegevens van [!DNL Audience Manager].

1. Bepaal publieksregels, dan selecteer **[!UICONTROL Save].**

>[!NOTE]
>
>U zou een inzicht in uw implementatievariabelen moeten hebben wanneer het bepalen van publieksregels.

Definieer onder [!UICONTROL Rules] de kenmerkselecties *`Home & Garden`*:

* **[!UICONTROL Attribute Source:]** Onbewerkte analysegegevens
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home & Garden]**

![](assets/home_garden.png)

De *Chrome &amp; Safari Bezoekers* is een publiekssegment dat wordt gedeeld door Analytics:

* **[!UICONTROL Attribute Source:]** Experience Cloud
* **[!UICONTROL Dimension:]** Chrome- en Safari-bezoekers

![](assets/chrome_safari.png)

Ter vergelijking kunt u een *OR*-regel toevoegen om alle bezoekers van een sitesectie, zoals Patio &amp; Furniture, te zien.

![](assets/audiences_rule_patio.png)

De resulterende regel is een gedefinieerd publiek bestaande uit gebruikers van Chrome en Safari die een bezoek hebben gebracht aan Home &amp; Garden. Het segment Patio &amp; Furniture biedt extra inzicht in alle bezoekers die dat gedeelte van de site bezoeken.

![](assets/defined_audience.png)

* **Historische schatting:** (gestippelde cirkel) geeft regels weer die zijn gemaakt op basis van  [!DNL Analytics] gegevens.
* **Werkelijk publiek:** (Ononderbroken cirkel) Om het even welke regel die 30 dagen van gegevens van Audience Manager heeft gecreeerd. Wanneer de gegevens van de Audience Manager 30 dagen bereiken, wordt de lijn stevig en vertegenwoordigt daadwerkelijke aantallen.

Nadat de gegevensinzameling voor de gespecificeerde periode voltooit, combineren de cirkels om een bepaald publiek te tonen.

Nadat het publiek wordt bewaard, is het beschikbaar voor andere oplossingen. U kunt bijvoorbeeld een gedeeld publiek opnemen in een Adobe Target-activiteit.
