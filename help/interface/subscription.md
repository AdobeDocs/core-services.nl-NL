---
description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van de Attributen van de Klant tussen de Experience Cloud en de toepassingen (Analytics en Doel) mogelijk.
solution: Experience Cloud
title: Hoe te om abonnementen te vormen
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Hoe te om abonnementen in Experience Cloud te vormen

Meer informatie over gegevensbronnen van toepassingen en abonnementen configureren. Abonnementen maken de gegevensstroom van Attributen van de Klant tussen Experience Cloud en toepassingen ([!DNL Analytics] en [!DNL Target]).

Met een Adobe Analytics-abonnement worden bijvoorbeeld kenmerkgegevens in rapporten ingeschakeld. Als u Adobe Target gebruikt, kunt u Klantkenmerken uploaden om ze als doel in te stellen en te segmenteren.

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL New]**

![Abonnementen configureren in Experience Cloud](assets/configure_subscription_page.png)

| Element | Beschrijving |
|--- |--- |
| Oplossing | **Adobe Analytics**<br> Selecteer Analytics, specificeer de rapportsuites aan dat u kenmerkgegevens wilt ontvangen, en de attributen om te omvatten.<br>**Adobe Target**<br> U kunt Klantkenmerken uploaden om ze te activeren en te segmenteren. Deze functie is handig als u een test wilt uitvoeren op basis van kenmerkgegevens of de gegevens beschikbaar wilt maken voor segmentatie in Analytics.<br>Geüploade kenmerkgegevens van de klant voor een bezoeker zijn beschikbaar bij aanmelding, in **[!DNL Target]** > **Soorten publiek**.<br>Meerdere gegevensbronnen worden ondersteund. Wanneer u  [klant-id&#39;s instellen](core-services.md) op uw website controleren of ten minste een van de aliassen is geabonneerd op [!DNL Target]. |
| Report Suite (Analytics) | Het rapport is afkomstig van Analytics.<br>U kunt niet meer dan een totaal van 10 rapportreeksen aan de abonnementen van Analytics binnen één enkele attributenbron toevoegen. Houd rekening met de volgende suggesties wanneer u kiest welke rapportsuites u wilt opnemen:<ul><li>Kies rapportsuites die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben. Als de voor authentiek verklaarde klanten in één rapportreeks niet met de voor authentiek verklaarde klanten in een andere rapportreeks overlappen, scheidt deze rapportreeksen in verschillende attributenbronnen.</li><li>Indien mogelijk, zouden de rapportreeksen inbegrepen in een attributenbron gelijkaardig verkeersvolume moeten hebben.</li></ul><br>Als u meer dan 10 rapportreeksen hebt die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben, kunt u extra bronnen van Attributen van de Klant vormen, elk met maximaal 10 rapportreeksen. |
| Te opnemen kenmerken (Analytics en [!DNL Target]) | De kenmerken die u naar de toepassing wilt verzenden. <br>Bij het configureren van abonnementen en het selecteren van kenmerken gelden de volgende limieten _per rapportenpakket,_ afhankelijk van de toepassingen die u hebt:<ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200 per rapportsuite</li><li>[!DNL Target] Standaard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Opmerking:** Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er aanvullende kenmerken beschikbaar zijn. U kunt een Max fout zien van het Abonnement van Attributen die tijdens deze vertraging wordt uitgegeven. |

{style=&quot;table-layout:auto&quot;}
