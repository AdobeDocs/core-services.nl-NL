---
title: '[!DNL Customer Attributes]'
description: Leer over  [!DNL Customer Attributes]  in Experience Cloud. Ontdek hoe u gegevens over klantkenmerken kunt uploaden voor gebruik in Adobe Analytics en Adobe Target.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
source-git-commit: fc60b49af0839769fdd8d18fd61863c8b28bbd57
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 5%

---

# [!DNL Customer Attributes] in Experience Cloud

[!DNL Customer Attributes] in Experience Cloud kunt u vastgelegde bedrijfsgegevens uploaden vanuit een CRM-database (Customer relationship management). U kunt de gegevens uploaden naar een gegevensbron voor klantkenmerken in Experience Cloud en vervolgens de gegevens in [!DNL Adobe Analytics] en [!DNL Adobe Target] gebruiken.

## De functie [!DNL Customer Attributes] zoeken

1. Login aan [!DNL Experience Cloud] en selecteert het menu ![ menu ](assets/menu-icon.png) pictogram.

1. Selecteer **[!DNL Customer Attributes]**.

![ overzicht van de attributen van de Klant ](assets/custom_reports.png)

## Vereisten voor het uploaden van klantkenmerkgegevens {#prerequisites}

* **het lidmaatschap van de Groep:** om de gegevens van de klantenattributen te uploaden, moeten de gebruikers lid van de groep van de Attributen van de Klant zijn. U moet ook tot een Adobe Analytics-groep of een Adobe Target-groep behoren.

  Om te weten of uw bedrijf toegang tot klantenattributen heeft, zou uw [!DNL Experience Cloud] beheerder in [ Experience Cloud ](https://experience.adobe.com) moeten registreren. Navigeer naar **[!UICONTROL Admin Console]** > **[!UICONTROL Products]** . Als *[!DNL Customer Attributes]* wordt weergegeven als een van de [!UICONTROL product profiles] , kunt u beginnen.

  Gebruikers die aan [!DNL Customer Attributes] zijn toegevoegd, zien de [!DNL Customer Attributes] -menuoptie aan de linkerkant van de Experience Cloud-interface.

* **Adobe Target** `at.js` (om het even welke versie) of `mbox.js` versie 58 of recenter wordt vereist voor klantenattributen.

  Zie [ hoe te om at.js ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html) op te stellen.

## Wat zijn bedrijfsklantgegevens? {#enterprise_data}

Bedrijfsgegevens bevinden zich in andere systemen. Het kan complex zijn en verschillende dingen betekenen voor verschillende mensen. Deze gegevens kunnen informatie omvatten zoals lidmaatschap, loyaliteitsniveau, leeftijd, geslacht, producten bezeten, belangen, en de Waarde van het Leven.

De volgende afbeelding is een voorbeeld van een gegevensbestand met abonneegegevens voor producten, waaronder id&#39;s van leden, producten met de naam, producten die het meest worden gestart, enzovoort.

![ wat gegevens van ondernemingsklanten is?](assets/01_crs_usecase.png)

Nadat u het gegevensbestand hebt gemaakt, kunt u het uploaden naar de kenmerkbron van de klant die u maakt in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer attributes]** .

Zie [ de gegevens van het klantenattribuut van de Upload ](t-crs-usecase.md) om dit werkschema te leren.

## Voorbeelden van klantkenmerken in Analytics en Target {#examples}

Nadat de gegevens in Experience Cloud zijn opgeslagen, kunt u deze aanpassen en delen met oplossingen voor rapportage, segmentatie, activiteiten en campagnes.

Bijvoorbeeld:

| Oplossing | Voordelen en gebruiksscenario&#39;s |
|--- |--- |
| Adobe Analytics | Marketers en analisten kunnen het volgende begrijpen:<ul><li>De online campagnes die het meest effectief zijn met uw klanten op goudniveau.</li><li>De producten die klanten op het niveau van goud naar tegenover producten zoeken die platina-vlakke klanten naar zoeken.</li><li>Of het herontwerp van uw site een positief effect heeft op de conversietarieven voor oudere klanten.</li><li>De producten die klanten met een lage levenwaarde neigen om op mijn plaats te onderzoeken.</li></ul> |
| Adobe Target | Met kenmerkgegevens kunnen Adobe Target-gebruikers:<ul><li>Speciale kortingen en aanbiedingen voor leden van loyaliteitsclubs weergeven.</li><li>U kunt duurdere producten aanbevelen aan uw luxe klanten.</li><li>Voor klanten die al e-mailberichten ontvangen, een up-sell-aanbieding weergeven in de ruimte die normaal gesproken is gereserveerd voor e-mailaanmelding</li></ul> |

{style="table-layout:auto"}
