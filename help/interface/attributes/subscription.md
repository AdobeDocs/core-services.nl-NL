---
description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van klantkenmerken tussen de Experience Cloud en oplossingen (Analytics en Target) mogelijk.
keywords: customer attributes;core services
seo-description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van klantkenmerken tussen de Experience Cloud en oplossingen (Analytics en Target) mogelijk.
seo-title: Abonnementen configureren
solution: Experience Cloud
title: Abonnementen configureren
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
translation-type: tm+mt
source-git-commit: b8363f024a09e07d26f6c0d0255e2675f7ef1a9a

---


# Abonnementen configureren

Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van klantkenmerken tussen de Experience Cloud en oplossingen (Analytics en Target) mogelijk.

Met een abonnement op Adobe Analytics worden bijvoorbeeld kenmerkgegevens in rapporten ingeschakeld. Als u Adobe Target gebruikt, kunt u klantkenmerken uploaden voor doelframes en segmentatie.

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL New]**

![](assets/configure_subscription_page.png)

| Element | Beschrijving |
|--- |--- |
| Oplossing | **Adobe **<br>AnalyticsSelect Analytics, specificeer de rapportsuites aan dat u kenmerkgegevens wilt ontvangen, en de attributen om te omvatten.<br>**Adobe**<br>TargetU kunt klantkenmerken uploaden voor doelframes en segmentatie. Deze functie is handig als u een test wilt uitvoeren op basis van kenmerkgegevens of de gegevens beschikbaar wilt maken voor segmentatie in Analytics.<br>Geüploade klantkenmerkgegevens voor een bezoeker zijn beschikbaar bij de aanmelding, in** Doel **>** Soorten publiek **.<br>Meerdere gegevensbronnen worden ondersteund. Wanneer u klant-id[&#39;s op uw website](../core-services/core-services.md)instelt, controleert u of ten minste een van de aliassen is geabonneerd op Target. |
| Report Suite (Analytics) | Het rapport is afkomstig van Analytics.<br>U kunt niet meer dan een totaal van 10 rapportreeksen aan de abonnementen van Analytics binnen één enkele attributenbron toevoegen. Houd rekening met de volgende suggesties wanneer u kiest welke rapportsuites u wilt opnemen:<ul><li>Kies rapportsuites die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben. Als de voor authentiek verklaarde klanten in één rapportreeks niet met de voor authentiek verklaarde klanten in een andere rapportreeks overlappen, scheidt deze rapportreeksen in verschillende attributenbronnen.</li><li>Indien mogelijk, zouden de rapportreeksen inbegrepen in een attributenbron gelijkaardig verkeersvolume moeten hebben.</li></ul><br>Als u meer dan 10 rapportreeksen hebt die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben, kunt u extra bronnen van klantenattributen vormen, elk met maximaal 10 rapportreeksen. |
| Te opnemen kenmerken (Analytics en Target) | De attributen die u naar de oplossing wilt verzenden. <br>Wanneer het vormen van abonnementen en het selecteren van attributen, zijn de volgende grenzen van toepassing _per rapportreeks,_ afhankelijk van de oplossingen u bezit:<ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200 per rapportsuite</li><li>Doelstandaard: 5</li><li>Doelpremie: 200</li></ul><br>**Opmerking:**Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er aanvullende kenmerken beschikbaar zijn. U kunt een Max fout zien van het Abonnement van Attributen die tijdens deze vertraging wordt uitgegeven. |
