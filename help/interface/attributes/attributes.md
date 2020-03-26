---
description: Overzicht en voorwaarden voor het uploaden van klantkenmerken naar de Experience Cloud.
keywords: core services;customer attributes
seo-description: Overzicht en voorwaarden voor het uploaden van klantkenmerken naar de Experience Cloud.
seo-title: Klantkenmerken
solution: Experience Cloud
title: Klantkenmerken
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Klantkenmerken

## Overzicht

Ga naar [!UICONTROL >] Personen **[!DNL Experience Platform]** > Kenmerken **[!UICONTROL klant om de]** klantkenmerken **[!UICONTROL te zoeken]**

Als u gegevens van ondernemingsklanten in een gegevensbestand van het het relatiebeheer van de klant (CRM) vangt, kunt u de gegevens in een gegevensbron van de klantenattributen in de Wolk van de Ervaring uploaden. Gebruik na het uploaden de gegevens in [!DNL Adobe Analytics] en [!DNL Adobe Target].

![](assets/custom_reports.png)

## Vereisten voor het uploaden van klantkenmerken {#section_BD38693AFBF34926BA28E964963B4EA0}


* **Oplossing ingeschakeld:** [Laat uw oplossingen voor de kerndiensten](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)toe.

* **Groepslidmaatschap:** Om klantkenmerkgegevens te uploaden, moeten de gebruikers lid van de groep [van Attributen van de](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9)Klant zijn. U moet ook deel uitmaken van een groep Adobe Analytics of een groep Adobe Target.

   Om te weten of uw bedrijf toegang tot klantenattributen heeft, zou uw [!DNL Experience Cloud] beheerder in het [!DNL Experience Cloud]moeten registreren. Ga naar **[!UICONTROL Beheer]** > **[!UICONTROL Admin Console]** starten > **[!UICONTROL Groepen]**. Als *Klantkenmerken* worden weergegeven als een van de groepen, kunt u beginnen.

   Gebruikers die aan de groep Kenmerken van klant worden toegevoegd, zien de menuoptie [!UICONTROL Klantenkenmerken] links in de interface van Experience Cloud.

* **Voor klantkenmerken is Adobe Target** [!DNL at.js] (elke versie) of [!DNL mbox.js] versie 58 of hoger vereist.


   Zie [hoe te om bij.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/deploy-at-js/how-to-deployatjs.html) of [Implementatie](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/mbox-download.html)Mbox.js op te stellen.

## Wat zijn bedrijfsklantgegevens? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Bedrijfsgegevens bevinden zich in andere systemen. Het kan complex zijn en verschillende dingen betekenen voor verschillende mensen. Deze gegevens kunnen informatie omvatten zoals lidmaatschap, loyaliteitsniveau, leeftijd, geslacht, producten bezeten, belangen, en de Waarde van het Leven.

De volgende afbeelding is een voorbeeld van een gegevensbestand met abonneegegevens voor producten, waaronder id&#39;s van leden, producten met de naam, producten die het meest worden gestart, enzovoort.

![](assets/01_crs_usecase.png)

Nadat u het gegevensbestand hebt gemaakt, kunt u het uploaden naar de bron van klantkenmerken die u maakt in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Klantkenmerken]**.

Zie [Klantkenmerkgegevens](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78) uploaden om deze workflow te leren.

## Gebruiksscenario&#39;s voor oplossing {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Nadat de gegevens zich in de Experience Cloud bevinden, kunt u deze aanpassen en delen met oplossingen voor rapportage, segmentatie, activiteiten en campagnes.

Bijvoorbeeld:

| Oplossing | Voordelen en gebruiksscenario&#39;s |
|--- |--- |
| Adobe Analytics | Marketers en analisten kunnen het volgende begrijpen:<ul><li>De online campagnes die het meest effectief zijn met uw klanten op goudniveau.</li><li>De producten die klanten op het niveau van goud naar tegenover producten zoeken die platina-vlakke klanten naar zoeken.</li><li>Of het herontwerp van uw site een positief effect heeft op de conversietarieven voor oudere klanten.</li><li>Welke producten klanten met een lage levenwaarde doen neigen aan onderzoek op mijn plaats.</li></ul> |
| Adobe-doel | Met kenmerkgegevens kunnen gebruikers van Adobe Target:<ul><li>Speciale kortingen en aanbiedingen voor leden van loyaliteitsclubs weergeven.</li><li>U kunt duurdere producten aanbevelen aan uw luxe klanten.</li><li>Voor klanten die al e-mailberichten ontvangen, een upsellatieaanbieding weergeven in de ruimte die normaal gesproken is gereserveerd voor e-mailhandtekeningen</li></ul> |
