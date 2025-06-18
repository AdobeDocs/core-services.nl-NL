---
description: Leer over de bronnen van oplossingsgegevens en het vormen abonnementen. Abonnementen maken de gegevensstroom van klantkenmerken tussen Experience Cloud en toepassingen (Analytics en Target) mogelijk.
solution: Experience Cloud
title: Hoe te om abonnementen te vormen
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Abonnementen configureren in Experience Cloud

Meer informatie over gegevensbronnen van toepassingen en abonnementen configureren. Abonnementen maken de [!DNL customer attribute] -gegevensstroom tussen Experience Cloud en toepassingen ([!DNL Analytics] en [!DNL Target] ) mogelijk.

Met een Adobe Analytics-abonnement worden bijvoorbeeld kenmerkgegevens in rapporten ingeschakeld. Als u Adobe Target gebruikt, kunt u klantkenmerken uploaden voor doelframes en segmentatie.

**[!UICONTROL customer attribute Source]** > **[!UICONTROL Create New customer attribute Source]** > **[!UICONTROL New]**

![ vorm abonnementen in Experience Cloud ](assets/configure_subscription_page.png)

| Element | Beschrijving |
|--- |--- |
| Oplossing | **<br>Uitgezocht van Adobe Analytics** [!DNL Analytics], specificeer de rapportsuites aan dat u kenmerkgegevens, en de attributen wilt ontvangen om te omvatten.<br>**Adobe Target**<br> U kunt klantenattributen voor het richten en segmentatie uploaden. Deze functie is handig als u een test wilt uitvoeren op basis van kenmerkgegevens of de gegevens beschikbaar wilt maken voor segmentatie in Analytics.<br> Geüploade gegevens van klantenattributen voor een bezoeker is beschikbaar bij login, in **[!DNL Target]** > **Soorten van publiek**.<br> de veelvoudige gegevensbronnen worden gesteund. Wanneer u klant-id&#39;s instelt op uw website, moet u controleren of ten minste een van de aliassen is geabonneerd op [!DNL Target] . |
| Rapportsuite (Adobe Analytics) | Het rapport is afkomstig van Analytics.<br> u kunt niet meer dan een totaal van 10 rapportreeksen aan de abonnementen van Analytics binnen één enkele attributenbron toevoegen. Houd rekening met de volgende suggesties wanneer u kiest welke rapportsuites u wilt opnemen:<ul><li>Kies rapportsuites die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben. Als de voor authentiek verklaarde klanten in één rapportreeks niet met de voor authentiek verklaarde klanten in een andere rapportreeks overlappen, scheidt deze rapportreeksen in verschillende attributenbronnen.</li><li>Indien mogelijk, zouden de rapportreeksen inbegrepen in een attributenbron gelijkaardig verkeersvolume moeten hebben.</li></ul><br> als u meer dan 10 rapportreeksen hebt die een gemeenschappelijke reeks voor authentiek verklaarde klanten hebben, kunt u extra bronnen van de klantenattributen vormen, elk met maximaal 10 rapportreeksen. |
| toe te voegen kenmerken (Analytics en [!DNL Target]) | De kenmerken die u naar de toepassing wilt verzenden. <br> wanneer het vormen van abonnementen en het selecteren van attributen, zijn de volgende grenzen _per rapportreeks van toepassing,_ afhankelijk van de toepassingen u bezit:<ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200 per rapportenpakket</li><li>[!DNL Target] Standaard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Nota:** wanneer u aan de Premium van Analytics bevordert, is er een vertraging van 24 uur alvorens de extra attributen beschikbaar zijn. U kunt een Max fout zien van het attributenabonnement tijdens deze vertraging. |

{style="table-layout:auto"}
