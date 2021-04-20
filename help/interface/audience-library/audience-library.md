---
solution: Experience Cloud
type: Documentation
title: 'Adobe Experience Cloud-publiek '
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
description: Leer hoe u de vertaling van bezoekersgegevens in publiekssegmentatie in de service Experience Cloud Audience beheert.
feature: Audience Library
topic: Administration
role: Administrator
level: Experienced
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 4%

---


# Experience Cloud publiek {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Soorten publiek zijn verzamelingen bezoekers (een lijst met bezoekers-id&#39;s). Met de Audience Library kunt u de omzetting van bezoekersgegevens in publiekssegmentatie beheren. Als dusdanig, is het creëren van, en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten. U kunt het publiekssegment aan producten en de diensten in [!DNL Experience Cloud] ook delen.

![](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe die in [!DNL Experience Cloud] worden gecreeerd
* [!DNL Analytics] segmenten gepubliceerd naar de  [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Real-Time versus Historisch publiek**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime doelwitten. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden elke 4 uur geëvalueerd. De totale verwerkings- en deeltijd kan maximaal 8 uur in beslag nemen. Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Het publiek in real time wordt afkomstig uit het publiek van de Experience Cloud en geëvalueerd in echt - tijd.

## Hoe oplossingen publiek {#concept_01EB9345C5344597BC94A864EDD38EE1} gebruiken

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in Experience Cloud-oplossingen:

| Oplossing | Beschrijving |
|--- |--- |
| Experience Cloud publiek | Creëer, beheer, en deel inheemse publiek gebruikend [de interface van de Bibliotheek van het publiek](../audience-library/audience-library.md). U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br>Voor suggesties over welk type publiek u wilt creëren zie:  [Experience Cloud publiek](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment aan Experience Cloud publiceren. Als u het segment publiceert, wordt dit op de pagina [!UICONTROL Audience Library] in Experience Cloud weergegeven. (Zie [Segmenten publiceren naar de Experience Cloud](https://docs.adobe.com/content/help/en/analytics/components/segmentation/segmentation-workflow/seg-publish.html) in de Help bij Analytics voor meer informatie.) Het publiek is ook beschikbaar als doelgroep voor een campagneervaring die door Adobe Target en in de Audience Manager wordt opgeleverd. Wanneer een publiek vanuit Adobe Analytics is gedeeld en is geselecteerd voor gebruik in een actieve campagne, worden alle bezoekersprofielen die de afgelopen 90 dagen aan de criteria voor segmentdefinitie voldeden, verzonden naar het Experience Cloud [!UICONTROL Audience Services]-platform. De grens voor gedeeld publiek is verhoogd tot 75. Het publiek dat vanuit Analytics aan de Experience Cloud wordt gedeeld, mag niet meer dan 20 miljoen unieke leden tellen. Vanwege caching is het bovendien 12 uur nodig voordat de verwijdering in de Experience Cloud wordt weergegeven. |
| Mobiele services | Analyseer mobiel verkeer gebruikend de zonnebarstvisualisatie in het [!UICONTROL Device Types] rapport. |
| [!DNL Target] | De [ID-service](https://docs.adobe.com/content/help/nl-NL/id-service/using/home.html) verenigt gebruikers-id&#39;s en gegevens in één actionabel profiel voor gebruik in verschillende oplossingen. Met het selectievakje [Publiceren naar de Experience Cloud](../audience-library/audience-library.md) tijdens het maken van segmenten in Adobe Analytics kan het segment beschikbaar zijn in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat in Analytics of Audience Manager wordt gecreeerd kan voor activiteiten in [!DNL Target] worden gebruikt. U kunt bijvoorbeeld campagneactiviteiten maken op basis van conversiemetriek [!DNL Analytics] en publiekssegmenten die zijn gemaakt in [!DNL Analytics]. |
| Audience Manager | Gedeeld publiek is beschikbaar in segmentatie van de Audience Manager. Alle Experience Cloud-soorten zijn in de Audience Manager verkrijgbaar, met:<ul><li>Ingebouwde automatisering betreffende hoe zij worden gedeeld en in oplossingswerkschema&#39;s verbruikt</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campaign | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-oplossingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-oplossingen die u gebruikt.</li></ul> |
| Advertising Cloud | Gebruik het publiek als doelen. |

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4-8 uur voordat die informatie in [!DNL Target], Ad Cloud en Campaign Standard kan worden uitgevoerd.

## Meer hulp - vragen, begeleiding en gebruiksgevallen {#section_C7F151644D8A45F7B6FC54F58845635D}

| Help met | Resource |
|--- |--- |
| Kan publiek niet vinden? | Zorg ervoor dat u provisioned bent. Zie [Aan de slag - uw oplossingen inschakelen voor kernservices](../core-services/core-services.md).<br>Klik  [](https://www.adobe.com/go/audiences) hier om toegang te vragen tot profielen en soorten publiek (inrichtingsformulier voor integraties). |
| Gebruiksscenario’s | Voor meer begeleiding op welke oplossing te gebruiken, ga naar [Opties van de Aanmaak van het publiek](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html) in de Kennisbank. |
| Forum | Het [Soorten publiek forum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) is een extra bron voor hulp bij het publiek. |

## Audiobabibliotheekinterface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

De [!DNL Experience Cloud] biedt een bibliotheek voor het maken en beheren van soorten publiek, met native, realtime publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![](assets/audience_library.png)

| Element | Beschrijving |
|--- |--- |
| Nieuw | [Een doelgroep maken](../audience-library/audience-library.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Bron | Identificeert waar het publiek is gemaakt.<ul><li>**Analytics:** Een segment dat in Adobe Analytics is gemaakt en vervolgens  [naar de Experience Cloud](../audience-library/audience-library.md) wordt gepubliceerd.</li><li>**Experience Cloud:** Een nieuw publiek  [gemaakt in Experience Cloud-publiek](../audience-library/audience-library.md).</li><li>**Audience Manager:Het** publiek creeerde Audience Manager toont automatisch in het publiek van de Experience Cloud.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |
