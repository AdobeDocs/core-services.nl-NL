---
description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. De abonnementen laten de gegevensstroom van de klantenattributen tussen de Experience Cloud en oplossingen (Analytics en Doel) toe.
keywords: Customer Attributes;core services
solution: Experience Cloud
title: 'Hoe te om abonnementen te vormen '
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


# Hoe te om abonnementen in Experience Cloud te vormen

Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. De abonnementen laten de gegevensstroom van de klantenattributen tussen de Experience Cloud en oplossingen (Analytics en [!DNL Target]) toe.

Met een Adobe Analytics-abonnement worden bijvoorbeeld kenmerkgegevens in rapporten ingeschakeld. Als u Adobe Target gebruikt, kunt u Klantkenmerken uploaden om ze als doel in te stellen en te segmenteren.

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL New]**

![](assets/configure_subscription_page.png)

| Element | Beschrijving |
|--- |--- |
| Oplossing | **Adobe**<br> AnalyticsSelect Analytics, specificeer de rapportsuites aan dat u kenmerkgegevens wilt ontvangen, en de attributen om te omvatten.<br>**Adobe**<br> TargetYou kan de Attributen van de Klant voor richten en segmentatie uploaden. Deze functie is handig als u een test wilt uitvoeren op basis van kenmerkgegevens of de gegevens beschikbaar wilt maken voor segmentatie in Analytics.<br>De geüploade klantkenmerkgegevens voor een bezoeker zijn beschikbaar bij de aanmelding, in **[!DNL Target]** > **Soorten publiek**.<br>Meerdere gegevensbronnen worden ondersteund. Wanneer u klant-id&#39;s [op uw website](../core-services/core-services.md) instelt, controleert u of ten minste een van de aliassen is geabonneerd op [!DNL Target]. |
| Report Suite (Analytics) | Het rapport is afkomstig van Analytics.<br>U kunt niet meer dan een totaal van 10 rapportreeksen aan de abonnementen van Analytics binnen één enkele attributenbron toevoegen. Houd rekening met de volgende suggesties wanneer u kiest welke rapportsuites u wilt opnemen:<ul><li>Kies rapportsuites die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben. Als de voor authentiek verklaarde klanten in één rapportreeks niet met de voor authentiek verklaarde klanten in een andere rapportreeks overlappen, scheidt deze rapportreeksen in verschillende attributenbronnen.</li><li>Indien mogelijk, zouden de rapportreeksen inbegrepen in een attributenbron gelijkaardig verkeersvolume moeten hebben.</li></ul><br>Als u meer dan 10 rapportreeksen hebt die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben, kunt u extra bronnen van klantenattributen vormen, elk met maximaal 10 rapportreeksen. |
| Te opnemen kenmerken (Analytics en [!DNL Target]) | De attributen die u naar de oplossing wilt verzenden. <br>Wanneer het vormen van abonnementen en het selecteren van attributen, zijn de volgende grenzen van toepassing _per rapportreeks,_ afhankelijk van de oplossingen u bezit:<ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200 per rapportsuite</li><li>[!DNL Target] Standaard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Opmerking:** Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er aanvullende kenmerken beschikbaar zijn. U kunt een Max fout zien van het Abonnement van Attributen die tijdens deze vertraging wordt uitgegeven. |
