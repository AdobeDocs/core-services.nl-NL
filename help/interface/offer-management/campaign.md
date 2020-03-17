---
description: Leer hoe u aanbiedingen kunt gebruiken en velden kunt delen in Adobe Campagne Standard.
seo-description: Leer hoe u aanbiedingen kunt gebruiken en velden kunt delen in Adobe Campagne Standard.
seo-title: Campagne
title: Campagne
uuid: ceeec50c-6441-4ced-915b-c73f349f7a21
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: a0e0b51d731343d5cd4226ab29d917aca63317c2

---


# Campagne{#campaign}

Leer hoe u aanbiedingen kunt gebruiken en velden kunt delen in Adobe Campagne Standard.

Nadat u ten minste één fallback-aanbieding en één algemene aanbieding hebt gemaakt, kunt u via een e-mail een aanbiedingsactiviteit maken in Campagnestandaard. Een aanbiedingsactiviteit kan slechts in een regelmatige e-mailcampagne worden gecreeerd. Deze kan niet worden toegevoegd aan een transactie-e-mailcampagne (bijvoorbeeld een terugkerende e-mail die wordt geactiveerd door een gebeurtenis, zoals een e-mailbericht om het winkelwagentje te verlaten).

Een aanbiedingsactiviteit zal u ertoe aanzetten om een groep voorstellen en een reserveaanbieding te selecteren die in een plaats in een e-mailmalplaatje zou kunnen worden getoond. De beste aanbieding die u kunt aanbieden, wordt geselecteerd op basis van de gegevens over plaatsing, datum, aanbiedingsstatus en klantprofiel tijdens het voorbereiden van de e-mail.

## Kenmerken delen van Campagne naar [!UICONTROL Offer Management]{#task_4DFA9A20D7B04E1F9AFF4774D67B6EBC}

Bij het maken van een aanbieding in [!UICONTROL Offer Management]kunt u subsidiabiliteitsregels instellen die beperken welke profielen bepaalde aanbiedingen kunnen ontvangen. Deze subsidiabiliteitsregels kunnen worden ingesteld op basis van kenmerken (of velden) die in het campagneprofiel voorkomen. Deze velden moeten worden gedeeld vanuit Campagne voordat ze worden weergegeven in de builder van de [!UICONTROL Offer Management] geschiktheidsregel.

>[!NOTE]
>
>Als u kenmerken wilt delen, moet u beheerdersrechten hebben in Campagne.

1. Klik **[!UICONTROL Adobe Campaign]** om navigatie te openen.
1. Navigeer naar **[!UICONTROL Administration]** > **[!UICONTROL Instance Settings]** > **[!UICONTROL Offer Management]** en klik **[!UICONTROL Attributes]**.

   Deze pagina bevat kenmerken die al zijn gedeeld. U kunt deze kenmerken bewerken of verwijderen.

   ![](assets/campaign-share5.png)

   >[!NOTE]
   >
   >Als een kenmerk momenteel wordt gebruikt door [!UICONTROL Offer Management] een toelatingsregel, kan het niet worden verwijderd.

1. Klik op **[!UICONTROL Create]**.

1. Klik op het mappictogram om de gegevensbron voor de campagne te definiëren en selecteer het element dat u wilt delen.

   ![](assets/campaign-share7.png)

1. Selecteer een label met doelgegevens.

   Dit is de naam voor het kenmerk dat wordt weergegeven in de builder van de geschiktheidsregel in [!UICONTROL Offer Management].

1. Klik op **[!UICONTROL Create]**.

   Het kenmerk wordt in de builder van de [!UICONTROL Offer Management] geschiktheidsregel weergegeven wanneer u aanbiedingen maakt en bewerkt.

   ![](assets/campaign-share2.png)

## Een aanbiedingsactiviteit maken {#task_F63ADDA52BD949779DB491E4D56E664E}

Voeg een aanbiedingsactiviteit in om het even welk beeld of tekstblok binnen een e-mailmalplaatje in de Norm van de Campagne in.

1. Als u een aanbiedingsactiviteit wilt invoegen op een afbeeldingslocatie, klikt u één keer op de afbeelding om het pictogram Voorstel invoegen weer te geven.

   ![](assets/insert-offer-activity.png)

1. (Alternatief): Als u een aanbiedingsactiviteit in een tekstblok wilt invoegen, klikt u tweemaal op het tekstblok om het pictogram Aanbieding invoegen te openen.

1. Vul de details in het [!UICONTROL Activity Details] lusje op het [!UICONTROL Create Offer Activity] scherm in:

   | Veld | Beschrijving |
   |---|---|
   | Naam activiteit | Geef uw activiteit een naam. Je kunt geen naam opgeven voor een activiteit die al in een andere aanbiedingsactiviteit is gebruikt. |
   | Plaatsing | Selecteer de plaatsing die voor deze plaats zal worden gebruikt. Zo zorgt u ervoor dat alleen aanbiedingen met een inhoudsweergave die overeenkomt met de plaatsing, aan een gebruiker worden aangeboden. Alleen aanbiedingen met deze plaatsing worden in de lijsten met aanbiedingen getoond gedurende de rest van de activiteit die wordt gemaakt. |

1. Selecteer op het [!UICONTROL Select Offers] tabblad de aanbiedingen die u in de activiteit wilt opnemen.

   U kunt groepen voorstellen selecteren met labels of afzonderlijke aanbiedingen een voor een.

   * **Groepen voorstellen selecteren met labels:**

      Als u groepen aanbiedingen met labels wilt selecteren, klikt u op het **[!UICONTROL Rule Builder]** tabblad en vervolgens op **[!UICONTROL Add Label Rule]**. Als u regels wilt maken om te bepalen welke aanbiedingen u wilt opnemen in de aanbiedingsactiviteit, selecteert u het label. Tussen de labels wordt een _EN_ -operator weergegeven. Als u de operator wilt wijzigen van _AND_ in _OR_, klikt u op de operator.

      ![](assets/offer-actvity-rule-builder.png)

   * **Afzonderlijke aanbiedingen selecteren:**

      Klik op het **[!UICONTROL Offer Inventory]** tabblad om afzonderlijke aanbiedingen te selecteren. Een gebruiker kan in de lijst met aanbiedingen zoeken op naam, aanbiedings-id of labels die aan de aanbieding zijn toegevoegd.

      Klik op het plusteken om de voorstellen toe te voegen aan de sectie Geselecteerde voorstellen in de lijst.

      ![](assets/create-offer2.png)

      Een voorstel is alleen beschikbaar in de ontwikkelaar van regels en in je aanbiedingsvoorraad als het:

   * Komt overeen met de datum van vandaag.
   * een erkend statuut hebben.
   * Zorg voor een inhoudsrepresentatie met een plaatsing die overeenkomt met de representatie die is geselecteerd in Stap 1.

      >[!NOTE]
      >
      >De voorstellen die op het tabblad Overzicht van aanbiedingen worden aangeboden, worden alleen gefilterd op basis van de status Plaatsing en Goedkeuring. Ze zijn niet gefilterd zodat ze voldoen aan de criteria voor het opgeven van doelen voor e-mail in Adobe Campaign.

1. Selecteer op het [!UICONTROL Fallback Offer] tabblad een fallback-aanbieding. De fallback-aanbieding wordt alleen naar een klant verzonden als deze niet in aanmerking komt voor andere aanbiedingen. U kunt slechts één fallback-aanbieding in de lijst selecteren.
1. Bekijk het overzicht van je aanbiedingsactiviteiten en klik op **[!UICONTROL Done]**.

   De beste aanbieding om elke gebruiker te dienen zal bij e-mailvoorbereiding door het volgende worden bepaald te evalueren:

* **Plaatsingscontrole:** Alle aanbiedingen moeten een inhoudsvertegenwoordiging hebben die de plaatsing als deel van de aanbiedingsactiviteit geselecteerde aanpast. Als een plaatsing voor een aanbieding tussen de tijd van de activiteitsschepping en voorbereidingstijd (als de tijd groter is dan drie minuten) wordt geschrapt, wordt die aanbieding niet overwogen.
* **Datum controle:** Alle aanbiedingen moeten geldig zijn voor de huidige datum (dit is _niet_ de verzenddatum van de aanbieding). De datum waarop u de e-mailcampagne voorbereidt, is de datum die bepaalt welke aanbieding moet worden uitgevoerd. Als u bijvoorbeeld op 1.15.17 een e-mailcampagne voorbereidt en een van de geselecteerde aanbiedingen pas 1.16.17 uur geldig is, wordt het voorstel niet verzonden.

* **Controle van de subsidiabiliteitsregel:** Alle aanbiedingen moeten voldoen aan de [subsidiabiliteitsregels](offers.md).

* **Prioriteitscontrole:** Als een gebruiker voor veelvoudige aanbiedingen in aanmerking komt, [!UICONTROL Offer Management] gebruikt de gebruiker-vastgestelde prioriteit om te bepalen welke aanbieding om elke gebruiker te tonen.

   Uw e-mail kan nu worden verzonden. Selecteer het [!UICONTROL Reports] tabblad op de [!DNL Adobe Campaign] homepage om te controleren hoe de aanbiedingen zijn uitgevoerd.

   Raadpleeg de volgende handleidingen voor meer informatie over het gebruik van Adobe Campaign:

* [Een e-mail maken](https://docs.campaign.adobe.com/doc/standard/en/CHA_Email_messages_Creating_an_email.html)
* [Een e-mail verzenden](https://docs.adobe.com/content/help/en/campaign-standard/using/testing-and-sending/about-sending-messages-with-campaign.html)
* [Dynamische rapporten](https://docs.campaign.adobe.com/doc/standard/en/RPT_About_reporting_About_dynamic_reports.html)

## Aanbiedingsrapporten

De Campagne van Adobe voorziet u van drie aanbiedingsdimensies (aanbieding, activiteit aan, aanbieding plaatsing) en één metrisch (aanbieding klikt) die u toestaan om uw aanbiedingen te controleren en hun effect te meten. Ga naar het tabblad Rapporten in Adobe Campagnestandaard om rapporten weer te geven. U kunt uw rapport creëren en verschillende aanbiedingsdimensies slepen en laten vallen in uw rapportpaneel beginnen uw gegevens te filtreren.

![](assets/offers-reports.png)

Zie [Informatie over dynamische rapporten](https://docs.campaign.adobe.com/doc/standard/en/RPT_About_reporting_About_dynamic_reports.html)voor meer informatie over het maken van dynamische rapporten in Campagne.