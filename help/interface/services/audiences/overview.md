---
title: "[!DNL Audience Library]"
description: Leer hoe te om de vertaling van bezoekersgegevens in publiekssegmentatie in Experience Cloud  [!DNL Audience Library] te beheren.
solution: Experience Cloud
type: Documentation
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: b257260bdbb7870dd6da807bceddfcddd2aef779
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 1%

---

# Experience Cloud publiek {#topic_679810123CAA4E0CA4FA3417FB0100C7}

In [!DNL Audience Library] wordt het publiek in het Experience Cloud weergegeven. Soorten publiek zijn verzamelingen bezoekers (een lijst met [!DNL Experience Cloud] id&#39;s). U kunt de vertaling van bezoekersgegevens in publiekssegmentatie beheren. Als zodanig lijkt het maken en beheren van soorten publiek op het maken en gebruiken van segmenten. U kunt het publiekssegment aan producten en de diensten in [!DNL Experience Cloud] ook delen.

![ Experience Cloud publiek ](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe in de [!DNL Experience Cloud] gemaakte
* [!DNL Analytics] segmenten gepubliceerd naar de [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Echte - tijd tegenover historisch publiek**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime doelwitten. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden om de vier uur geëvalueerd. De totale tijd om te verwerken en te delen duurt tot acht uur. Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Het publiek in real time wordt teruggebracht tot publiek van het Experience Cloud en in echt - tijd geëvalueerd.

## Hoe toepassingen publiek gebruiken {#concept_01EB9345C5344597BC94A864EDD38EE1}

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in toepassingen voor Experiencen Cloud:

| Oplossing | Beschrijving |
|--- |--- |
| Experience Cloud-doelgroepen | Maak, beheer en deel publiek native met behulp van Audience Library. U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br> voor suggesties over welk type van publiek u wilt tot stand brengen zie [ de schepingsopties van het Publiek ](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html). |
| Analytics | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment aan Experience Cloud publiceren. Als u het segment publiceert, wordt dit op de [!DNL Audience Library] -pagina in Experience Cloud weergegeven. (Zie [ de segmenten van Publish aan Experience Cloud ](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html) in [!DNL Analytics] hulp voor details.) Het publiek is ook beschikbaar als doelgroep voor een campagneervaring die wordt geleverd door [!DNL Adobe Target] en in [!DNL Audience Manager] . Nadat u een publiek van [!DNL Adobe Analytics] deelt, en het voor gebruik in een actieve campagne selecteert, worden de bezoekersprofielen die aan de criteria van de segmentdefinitie voor de afgelopen 90 dagen voldoen verzonden naar [!UICONTROL Audience Services]. De grens voor gedeeld publiek is verhoogd tot 75. Soorten publiek dat vanuit [!DNL Analytics] aan Experience Cloud wordt gedeeld, mogen niet meer dan 20 miljoen unieke leden bevatten. Vanwege caching is het bovendien 12 uur nodig voordat de verwijdering in het Experience Cloud wordt weergegeven. |
| Mobiele services | Analyseer mobiel verkeer met gebruik van de zonneexplosie-visualisatie in het [!UICONTROL Device Types] -rapport. |
| [!DNL Target] | De [ dienst van identiteitskaart ](https://experienceleague.adobe.com/docs/id-service/using/home.html) verenigt bezoeker IDs en gegevens in één enkel, actionable profiel voor gebruik over toepassingen. Met het selectievakje [!UICONTROL Publish to Experience Cloud] tijdens het maken van segmenten in Adobe Analytics kan het segment beschikbaar zijn in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat is gemaakt in [!DNL Analytics] of [!DNL Audience Manager] , kan worden gebruikt voor activiteiten in [!DNL Target] . U kunt bijvoorbeeld campagneactiviteiten maken op basis van [!DNL Analytics] conversiemetriek en publiekssegmenten die zijn gemaakt in [!DNL Analytics] . |
| [!DNL Audience Manager] | Gedeeld publiek is beschikbaar in [!DNL Audience Manager] segmentatie. Alle soorten publiek in het Experience Cloud zijn native beschikbaar in [!DNL Audience Manager] , dat het volgende biedt:<ul><li>Ingebouwde automatisering voor de manier waarop ze worden gedeeld en verbruikt in workflows van toepassingen</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campaign | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-toepassingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-toepassingen die u gebruikt.</li></ul> |
| Advertising Cloud | Gebruik het publiek als doelen. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4-8 uur voordat die informatie in [!DNL Target] , Ad Cloud en Campaign Standard kan worden uitgevoerd.

## Audio Library-interface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

[!DNL Experience Cloud] verstrekt een bibliotheek voor het creëren van en het leiden van publiek, met inheemse, real-time publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![ voeg publiek in de Bibliotheek van het Publiek toe ](assets/audience_library.png)


| Element | Beschrijving |
|--- |--- |
| Nieuw | [ creeer een publiek ](create.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Source | Identificeert waar het publiek is gemaakt.<ul><li>**Analytics:** een segment dat in Adobe Analytics wordt gecreeerd, dan aan Experience Cloud wordt gepubliceerd.</li><li>**Experience Cloud:** een nieuw publiek [ dat in het Soorten publiek van het Experience Cloud ](create.md) wordt gecreeerd.</li><li>**Audience Manager:** het publiek creeerde automatisch de vertoning van de Audience Manager in het Soorten publiek van het Experience Cloud.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |

{style="table-layout:auto"}

## Publish-publiek uit Adobe Analytics

Zie [ de segmenten van Publish aan Experience Cloud ](https://experienceleague.adobe.com/en/docs/analytics/components/segmentation/segmentation-workflow/seg-publish) in de documentatie van Adobe Analytics voor meer informatie.
