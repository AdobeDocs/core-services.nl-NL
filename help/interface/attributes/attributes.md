---
description: Leer meer over de Customer Attributes-service in Adobe Experience Cloud en hoe u de gegevens uploadt voor gebruik in Analytic and Target.
keywords: core services;Customer Attributes; Adobe Experience Cloud; Analytics; Target
solution: Experience Cloud
title: 'Hoe te om de Attributen van de Klant te gebruiken '
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---


# Klantkenmerken gebruiken in Adobe Experience Cloud

De Attributen van de klant in Adobe Experience Cloud laten u toe om uw gevangen ondernemingsgegevens van een gegevensbestand van het het relatiebeheer van de klant (CRM) te uploaden. U kunt de gegevens uploaden naar een gegevensbron voor klantkenmerken in de Experience Cloud en vervolgens de gegevens in Adobe Analytics en Adobe Target gebruiken.

Navigeer naar **[!DNL Experience Platform]** > **[!UICONTROL People]** > om deze functie te zoeken. **[!UICONTROL Customer Attributes]**

![](assets/custom_reports.png)

## Vereisten voor het uploaden van klantkenmerken {#section_BD38693AFBF34926BA28E964963B4EA0}

* **Oplossing ingeschakeld:** [Laat uw oplossingen voor de diensten](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)van het Experience Platform toe.

* **Groepslidmaatschap:** Gebruikers die klantkenmerkgegevens willen uploaden, moeten lid zijn van de groep [](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9)Klantkenmerken. U moet ook tot een Adobe Analytics-groep of een Adobe Target-groep behoren.

   Om te weten of uw bedrijf toegang tot de Attributen van de Klant heeft, zou uw [!DNL Experience Cloud] beheerder zich in de [Experience Cloud](https://experience.adobe.com)moeten aanmelden. Ga naar **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. Als *Klantkenmerken* als een van de [!UICONTROL Product Profiles]kenmerken worden weergegeven, kunt u beginnen.

   De gebruikers die aan de Attributen van de Klant worden toegevoegd zullen het [!UICONTROL Customer Attributes] menupunt op de linkerkant van de interface van Experience Cloud zien.

* **Adobe Target** `at.js` (elke versie) of `mbox.js` versie 58 of hoger is vereist voor Klantkenmerken.

   Zie [hoe te om bij.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/deploy-at-js/how-to-deployatjs.html) of [Implementatie](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/mbox-download.html)Mbox.js op te stellen.

## Wat zijn bedrijfsklantgegevens? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Bedrijfsgegevens bevinden zich in andere systemen. Het kan complex zijn en verschillende dingen betekenen voor verschillende mensen. Deze gegevens kunnen informatie omvatten zoals lidmaatschap, loyaliteitsniveau, leeftijd, geslacht, producten bezeten, belangen, en de Waarde van het Leven.

De volgende afbeelding is een voorbeeld van een gegevensbestand met abonneegegevens voor producten, waaronder id&#39;s van leden, producten met de naam, producten die het meest worden gestart, enzovoort.

![](assets/01_crs_usecase.png)

Nadat u het gegevensbestand hebt gemaakt, kunt u het uploaden naar de bron van klantkenmerken die u maakt in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer Attributes]**.

Zie [Klantkenmerkgegevens](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78) uploaden om deze workflow te leren.

## Voorbeelden van klantkenmerken in Analytics en Target {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Nadat de gegevens in de Experience Cloud verblijven, kunt u het aanpassen en het aan oplossingen voor rapportering, segmentatie, activiteiten, en campagnes delen.

Bijvoorbeeld:

| Oplossing | Voordelen en gebruiksscenario&#39;s |
|--- |--- |
| Adobe Analytics | Marketers en analisten kunnen het volgende begrijpen:<ul><li>De online campagnes die het meest effectief zijn met uw klanten op goudniveau.</li><li>De producten die klanten op het niveau van goud naar tegenover producten zoeken die platina-vlakke klanten naar zoeken.</li><li>Of het herontwerp van uw site een positief effect heeft op de conversietarieven voor oudere klanten.</li><li>Welke producten klanten met een lage levenwaarde doen neigen aan onderzoek op mijn plaats.</li></ul> |
| Adobe Target | Met kenmerkgegevens kunnen Adobe Target-gebruikers:<ul><li>Speciale kortingen en aanbiedingen voor leden van loyaliteitsclubs weergeven.</li><li>U kunt duurdere producten aanbevelen aan uw luxe klanten.</li><li>Voor klanten die al e-mailberichten ontvangen, een up-sell-aanbieding weergeven in de ruimte die normaal gesproken is gereserveerd voor e-mailaanmelding</li></ul> |
