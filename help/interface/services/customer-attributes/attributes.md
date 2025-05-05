---
title: "[!DNL Customer Attributes]"
description: Leer over  [!DNL Customer Attributes]  in Experience Cloud. Ontdek hoe u gegevens voor klantkenmerken kunt uploaden voor gebruik in Adobe Analytics en Adobe Target.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 5%

---

# [!DNL Customer Attributes] in Experience Cloud

[!DNL Customer Attributes] in Experience Cloud biedt u de mogelijkheid om uw vastgelegde bedrijfsgegevens te uploaden vanuit een CRM-database (customer relationship management). U kunt de gegevens uploaden naar een gegevensbron voor klantkenmerken in Experience Cloud en vervolgens de gegevens in [!DNL Adobe Analytics] en [!DNL Adobe Target] gebruiken.

## De functie [!DNL Customer Attributes] zoeken

1. Meld u aan bij het Experience Cloud.

1. Navigeer naar **[!DNL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]** .

![ Overzicht van de Attributen van de Klant ](assets/custom_reports.png)

## Vereisten voor uploaden [!DNL Customer Attributes] {#section_BD38693AFBF34926BA28E964963B4EA0}

* **het lidmaatschap van de Groep:** om de gegevens van Attributen van de Klant te uploaden, moeten de gebruikers lid van de groep van Attributen van de Klant zijn. U moet ook tot een Adobe Analytics-groep of een Adobe Target-groep behoren.

  Om te weten of uw bedrijf toegang tot de Attributen van de Klant heeft, zou uw [!DNL Experience Cloud] beheerder in het [ Experience Cloud ](https://experience.adobe.com) moeten registreren. Ga naar **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. Als *[!DNL Customer Attributes]* wordt weergegeven als een van de [!UICONTROL product profiles] , kunt u beginnen.

  Gebruikers die aan [!DNL Customer Attributes] worden toegevoegd, zien het [!UICONTROL Customer Attributes] menu-item links van de interface van het Experience Cloud.

* **Adobe Target** `at.js` (om het even welke versie) of `mbox.js` versie 58 of recenter wordt vereist voor de Attributen van de Klant.

  Zie [ hoe te om at.js ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html?lang=nl-NL) op te stellen.

## Wat zijn bedrijfsklantgegevens? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Bedrijfsgegevens bevinden zich in andere systemen. Het kan complex zijn en verschillende dingen betekenen voor verschillende mensen. Deze gegevens kunnen informatie omvatten zoals lidmaatschap, loyaliteitsniveau, leeftijd, geslacht, producten bezeten, belangen, en de Waarde van het Leven.

De volgende afbeelding is een voorbeeld van een gegevensbestand met abonneegegevens voor producten, waaronder id&#39;s van leden, producten met de naam, producten die het meest worden gestart, enzovoort.

![ wat gegevens van ondernemingsklanten is?](assets/01_crs_usecase.png)

Nadat u het gegevensbestand creeert, kunt u het aan de bron van Attributen van de Klant uploaden die u in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer Attributes]** creeert.

Zie [ gegevens van het Attribuut van de Klant uploaden ](t-crs-usecase.md) om dit werkschema te leren.

## Voorbeelden van klantkenmerken in Analytics en Target {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Nadat de gegevens in Experience Cloud verblijven, kunt u het aanpassen en het aan oplossingen voor rapportering, segmentatie, activiteiten, en campagnes delen.

Bijvoorbeeld:

| Oplossing | Voordelen en gebruiksscenario&#39;s |
|--- |--- |
| Adobe Analytics | Marketers en analisten kunnen het volgende begrijpen:<ul><li>De online campagnes die het meest effectief zijn met uw klanten op goudniveau.</li><li>De producten die klanten op het niveau van goud naar tegenover producten zoeken die platina-vlakke klanten naar zoeken.</li><li>Of het herontwerp van uw site een positief effect heeft op de conversietarieven voor oudere klanten.</li><li>De producten die klanten met een lage levenwaarde neigen om op mijn plaats te onderzoeken.</li></ul> |
| Adobe Target | Met kenmerkgegevens kunnen Adobe Target-gebruikers:<ul><li>Speciale kortingen en aanbiedingen voor leden van loyaliteitsclubs weergeven.</li><li>U kunt duurdere producten aanbevelen aan uw luxe klanten.</li><li>Voor klanten die al e-mailberichten ontvangen, een up-sell-aanbieding weergeven in de ruimte die normaal gesproken is gereserveerd voor e-mailaanmelding</li></ul> |

{style="table-layout:auto"}
