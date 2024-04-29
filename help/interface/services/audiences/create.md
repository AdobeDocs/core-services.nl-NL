---
description: Leer hoe u kenmerkregels gebruikt om een publiek te maken en een samengesteld publiek in Adobe Experience Cloud te definiëren.
solution: Experience Cloud
title: Een publiek maken
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Een publiek maken

Leer hoe te om attributenregels te gebruiken om een publiek tot stand te brengen en een samengesteld publiek in Experience Cloud te bepalen.

Dit artikel helpt u begrijpen hoe te:

* Een publiek maken
* Een regel maken
* Regels gebruiken om een samengesteld publiek te definiëren

De volgende afbeelding vertegenwoordigt twee regels in een samengesteld publiek.

![Twee regels in een samengesteld publiek](assets/audience_sharing.png)

Elke cirkel vertegenwoordigt een regel die publiekslidmaatschap bepaalt. Bezoekers die als leden in beide publieksregels worden gekwalificeerd, overlappen elkaar om het samengestelde, gedefinieerde publiek te worden.

>[!NOTE]
>
>Het publiek wordt volledig gedefinieerd nadat de gegevensverzameling voor de opgegeven periode is voltooid.

In het volgende voorbeeld ziet u hoe u de regels voor een samengesteld publiek maakt. Dit publiek bestaat uit:

* De sectie Home &amp; Garden is afgeleid van paginagegevens of onbewerkte analysegegevens.
* Chrome- en Safari-gebruikers afgeleid van een [!DNL Adobe Analytics] segment [gepubliceerd](overview.md) aan de [!DNL Experience Cloud].

  ![De regels voor een samengesteld publiek maken](assets/audience_create.png)

**Een publiek maken**

1. In de [!DNL Experience Cloud], onder [!DNL Experience Platform], selecteert u **[!UICONTROL People]** > **[!UICONTROL Audience Library].**
1. Op de [!UICONTROL Audiences] pagina, selecteert u **[!UICONTROL New]**. ![toevoegen](assets/add_icon_small.png)

   ![Stap Resultaat](assets/audience_create_new.png)

1. Op de [!UICONTROL Create New Audience] , geeft u een titel en beschrijving op.
1. Onder [!UICONTROL Rules]selecteert u een kenmerkbron:

   * **[!UICONTROL Real-Time Analytics Data:]** (of Raw-gegevens) Dit zijn kenmerkgegevens die zijn afgeleid van Real-Time Analytics-afbeeldingsaanvragen en die gegevens bevatten zoals eVars en gebeurtenissen. U moet een rapportreeks selecteren wanneer het gebruiken van deze attributenbron, en de dimensie of de gebeurtenis bepalen om te omvatten. Deze selectie van de rapportreeks verstrekt de veranderlijke structuur die door de rapportreeks wordt gebruikt.
   >[!NOTE]
   >
   >Als gevolg van caching, vereisen de geschrapte rapportreeksen in Analytics 12 uur alvorens de schrapping in Experience Cloud wordt getoond.

   * **[!UICONTROL Experience Cloud:]** Kenmerkgegevens die zijn afgeleid van de [!DNL Experience Cloud] bronnen. Dit kunnen bijvoorbeeld gegevens zijn van publiekssegmenten waarin u creeert [!DNL Analytics]of gegevens van [!DNL Audience Manager].

1. Bepaal publieksregels, dan selecteer **[!UICONTROL Save].**

>[!NOTE]
>
>U zou een inzicht in uw implementatievariabelen moeten hebben wanneer het bepalen van publieksregels.

Onder [!UICONTROL Rules], de *`Home & Garden`* kenmerkselecties:

* **[!UICONTROL Attribute Source:]** Onbewerkte analysegegevens
* **[!UICONTROL Report Suite:]** Report Suite 31
* DIMENSION = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home & Garden]**

![Kenmerkselecties in Audience Library](assets/home_garden.png)

De *Chrome- en Safari-bezoekers* is een publiekssegment dat wordt gedeeld door Analytics:

* **[!UICONTROL Attribute Source:]** Experience Cloud
* **[!UICONTROL Dimension:]** Chrome- en Safari-bezoekers

![Chrome- en Safari-bezoekers](assets/chrome_safari.png)

Ter vergelijking kunt u een *OF* om alle bezoekers van een sitesectie, zoals Patio &amp; Furniture, te zien.

![OR-regel voor een publiek](assets/audiences_rule_patio.png)

De resulterende regel is een gedefinieerd publiek bestaande uit gebruikers van Chrome en Safari die een bezoek hebben gebracht aan Home &amp; Garden. Het segment Patio &amp; Furniture biedt extra inzicht in alle bezoekers die dat gedeelte van de site bezoeken.

![Gedefinieerd publiek in Experience Cloud](assets/defined_audience.png)

* **Historische schatting:** (Stippelcirkel) Geeft regels weer die zijn gemaakt op basis van [!DNL Analytics] gegevens.
* **Werkelijk publiek:** (Ononderbroken cirkel) Elke regel die is gemaakt en die 30 dagen gegevens uit Audience Manager bevat. Wanneer de gegevens van de Audience Manager 30 dagen bereiken, wordt de lijn stevig en vertegenwoordigt daadwerkelijke aantallen.

Nadat de gegevensinzameling voor de gespecificeerde periode voltooit, combineren de cirkels om een bepaald publiek te tonen.

Nadat het publiek is opgeslagen, is het beschikbaar voor andere toepassingen. U kunt bijvoorbeeld een gedeeld publiek opnemen in een Adobe Target-activiteit.
