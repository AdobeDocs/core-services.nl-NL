---
description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van Kenmerken van de Klant tussen Experience Cloud en toepassingen (Analytics en Target) mogelijk.
solution: Experience Cloud
title: Abonnementen configureren
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Hoe te om abonnementen in Experience Cloud te vormen

Meer informatie over gegevensbronnen van toepassingen en abonnementen configureren. Abonnementen maken de [!DNL Customer Attribute] gegevensstroom tussen Experience Cloud en toepassingen ([!DNL Analytics] en [!DNL Target]) mogelijk.

Met een Adobe Analytics-abonnement worden bijvoorbeeld kenmerkgegevens in rapporten ingeschakeld. Als u Adobe Target gebruikt, kunt u Klantkenmerken uploaden om deze te activeren en te segmenteren.

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL New]**

![ vorm abonnementen in Experience Cloud ](assets/configure_subscription_page.png)

| Element | Beschrijving |
|--- |--- |
| Oplossing | **<br>Uitgezocht van Adobe Analytics** [!DNL Analytics], specificeer de rapportsuites aan dat u kenmerkgegevens, en de attributen wilt ontvangen om te omvatten.<br>**Adobe Target**<br> U kunt de Attributen van de Klant voor het richten en segmentatie uploaden. Deze functie is handig als u een test wilt uitvoeren op basis van kenmerkgegevens of de gegevens beschikbaar wilt maken voor segmentatie in Analytics.<br> Geüploade gegevens van de Attributen van de Klant voor een bezoeker is beschikbaar bij login, in **[!DNL Target]** > **Soorten van publiek**.<br> de veelvoudige gegevensbronnen worden gesteund. Wanneer u klant-id&#39;s instelt op uw website, moet u controleren of ten minste een van de aliassen is geabonneerd op [!DNL Target] . |
| Report Suite (Analytics) | Het rapport is afkomstig van Analytics.<br> u kunt niet meer dan een totaal van 10 rapportreeksen aan de abonnementen van Analytics binnen één enkele attributenbron toevoegen. Houd rekening met de volgende suggesties wanneer u kiest welke rapportsuites u wilt opnemen:<ul><li>Kies rapportsuites die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben. Als de voor authentiek verklaarde klanten in één rapportreeks niet met de voor authentiek verklaarde klanten in een andere rapportreeks overlappen, scheidt deze rapportreeksen in verschillende attributenbronnen.</li><li>Indien mogelijk, zouden de rapportreeksen inbegrepen in een attributenbron gelijkaardig verkeersvolume moeten hebben.</li></ul><br> als u meer dan 10 rapportreeksen hebt die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben, kunt u de extra bronnen van Attributen van de Klant vormen, elk met maximaal 10 rapportreeksen. |
| Te opnemen kenmerken (Analytics en [!DNL Target]) | De kenmerken die u naar de toepassing wilt verzenden. <br> wanneer het vormen van abonnementen en het selecteren van attributen, zijn de volgende grenzen _per rapportreeks van toepassing,_ afhankelijk van de toepassingen u bezit:<ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200 per rapportenpakket</li><li>[!DNL Target] Standaard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Nota:** wanneer u aan de Premium van Analytics bevordert, is er een vertraging van 24 uur alvorens de extra attributen beschikbaar zijn. U kunt een Max fout zien van het Abonnement van Attributen die tijdens deze vertraging wordt uitgegeven. |

{style="table-layout:auto"}
