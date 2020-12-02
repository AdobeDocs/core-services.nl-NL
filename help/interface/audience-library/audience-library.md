---
description: Leer hoe u de vertaling van bezoekersgegevens naar publiekssegmentatie in de Adobe Experience Cloud Audience-service beheert.
seo-description: Beheer de vertaling van bezoekersgegevens in publiekssegmentatie in de dienst van het Experience Cloud publiek.
seo-title: Experience Cloud-publiek
solution: Experience Cloud
title: 'Adobe Experience Cloud-publiek '
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: tm+mt
source-git-commit: e7d297820dbb666308c5906eca01a0c248e35fe3
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 4%

---


# Experience Cloud Audiences {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Soorten publiek zijn verzamelingen bezoekers (een lijst met bezoekers-id&#39;s). Met de Audience Library kunt u de omzetting van bezoekersgegevens in publiekssegmentatie beheren. Als dusdanig, is het creëren van, en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten. U kunt het publiekssegment aan producten en de diensten in ook delen [!DNL Experience Cloud].

![](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe in het dialoogvenster [!DNL Experience Cloud]
* [!DNL Analytics] segmenten gepubliceerd naar de [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Real-Time versus Historisch publiek**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime doelwitten. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden elke 4 uur geëvalueerd. De totale verwerkings- en deeltijd kan maximaal 8 uur in beslag nemen. Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Het publiek in real time wordt afkomstig uit het publiek van de Experience Cloud en geëvalueerd in echt - tijd.

## Hoe oplossingen publiek gebruiken {#concept_01EB9345C5344597BC94A864EDD38EE1}

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in Experience Cloud-oplossingen:

| Oplossing | Beschrijving |
|--- |--- |
| Experience Cloud publiek | Maak, beheer en deel publiek native met behulp van de interface [Audience Library](../audience-library/audience-library.md) . U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br>Voor suggesties over welk type publiek u wilt creëren zie: [Experience Cloud publiek](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment aan Experience Cloud publiceren. Als u het segment publiceert, wordt dit op de [!UICONTROL Audience Library] pagina in Experience Cloud weergegeven. (Zie Segmenten [publiceren naar de Experience Cloud](https://docs.adobe.com/content/help/en/analytics/components/segmentation/segmentation-workflow/seg-publish.html) in de Help bij Analytics voor meer informatie.) Het publiek is ook beschikbaar als doelgroep voor een campagneervaring die door Adobe Target en in de Audience Manager wordt opgeleverd. Wanneer een publiek vanuit Adobe Analytics wordt gedeeld en wordt geselecteerd voor gebruik in een actieve campagne, worden alle bezoekersprofielen die de afgelopen 90 dagen aan de criteria voor segmentdefinitie voldeden, naar het Experience Cloud- [!UICONTROL Audience Services] platform verzonden. De grens voor gedeeld publiek is verhoogd tot 75. Het publiek dat vanuit Analytics aan de Experience Cloud wordt gedeeld, mag niet meer dan 20 miljoen unieke leden tellen. Vanwege caching is het bovendien 12 uur nodig voordat de verwijdering in de Experience Cloud wordt weergegeven. |
| Mobiele services | Analyseer mobiel verkeer gebruikend de zonnebarstvisualisatie in het [!UICONTROL Device Types] rapport. |
| [!DNL Target] | Met de [id-service](https://docs.adobe.com/content/help/nl-NL/id-service/using/home.html) verenigt u gebruikers-id&#39;s en gegevens in één actionabel profiel voor gebruik in verschillende oplossingen. Met het selectievakje [Publiceren naar Experience Cloud](../audience-library/audience-library.md) tijdens het maken van segmenten in Adobe Analytics kan het segment beschikbaar zijn in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat in Analytics of Audience Manager wordt gecreeerd kan voor activiteiten in worden gebruikt [!DNL Target]. U kunt bijvoorbeeld campagneactiviteiten maken op basis van [!DNL Analytics] conversiemetriek en publiekssegmenten die zijn gemaakt in [!DNL Analytics]. |
| Audience Manager | Gedeeld publiek is beschikbaar in segmentatie van de Audience Manager. Alle Experience Cloud-soorten zijn in de Audience Manager verkrijgbaar, met:<ul><li>Ingebouwde automatisering betreffende hoe zij worden gedeeld en in oplossingswerkschema&#39;s verbruikt</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campaign | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-oplossingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-oplossingen die u gebruikt.</li></ul> |
| Media optimaliseren | Gebruik het publiek als doelen. |

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4-8 uur voordat die informatie in [!DNL Target], Ad Cloud en Campaign Standard kan worden uitgevoerd.

## Meer hulp - vragen, begeleiding en gebruiksgevallen {#section_C7F151644D8A45F7B6FC54F58845635D}

| Help met | Resource |
|--- |--- |
| Kan publiek niet vinden? | Zorg ervoor dat u provisioned bent. Zie [Aan de slag - stel uw oplossingen in voor de kernservices](../core-services/core-services.md).<br>Klik [hier](https://www.adobe.com/go/audiences) om toegang te vragen tot profielen en soorten publiek (inrichtingsformulier voor integraties). |
| Gebruiksscenario’s | Voor meer begeleiding op welke oplossing te gebruiken, ga naar de Opties [van de Aanmaak van het](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html) publiek in de Kennisbank. |
| Forum | Het [Soortforum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) is een extra bron voor hulp bij het publiek. |

## Audio Library-interface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

Het [!DNL Experience Cloud] biedt een bibliotheek voor het maken en beheren van publiek, met native, realtime publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![](assets/audience_library.png)

| Element | Beschrijving |
|--- |--- |
| Nieuw | [Een doelgroep maken](../audience-library/audience-library.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Bron | Identificeert waar het publiek is gemaakt.<ul><li>**Analyse:** Een segment gemaakt in Adobe Analytics en vervolgens [gepubliceerd naar de Experience Cloud](../audience-library/audience-library.md).</li><li>**Experience Cloud:** Een nieuw publiek [gemaakt in het Experience Cloud publiek](../audience-library/audience-library.md).</li><li>**Audience Manager:** Het publiek creeerde Audience Manager toont automatisch in het Publiek van de Experience Cloud.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |
