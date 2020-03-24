---
description: De vertaling van bezoekersgegevens in publiekssegmentatie beheren.
seo-description: De vertaling van bezoekersgegevens in publiekssegmentatie beheren.
seo-title: Soorten publiek
solution: Experience Cloud
title: Soorten publiek
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: tm+mt
source-git-commit: 14d6e0ae15b023ad4dd3f8aca0606f26b39a21e9

---


# Audiences {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Soorten publiek zijn verzamelingen bezoekers (een lijst met bezoekers-id&#39;s). De publieksservices van Adobe beheren de vertaling van bezoekersgegevens naar publiekssegmentatie. Als dusdanig, is het creëren van en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten, met de toegevoegde capaciteit om het publiekssegment aan [!DNL Experience Cloud]te delen.

![](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe in het dialoogvenster [!DNL Experience Cloud]
* Van [!DNL Analytics] segmenten gepubliceerd naar [!DNL Experience Cloud]
* Van [!DNL Audience Manager]

**Real-Time vs. Historische doelgroepen**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime-doelen. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden elke 4 uur geëvalueerd. De totale verwerkings- en deeltijd kan maximaal 8 uur in beslag nemen.  Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Echte-tijdpubliek wordt betrokken bij de Experience Cloud Audiences en wordt in real-time geëvalueerd.

## Hoe oplossingen publiek gebruiken {#concept_01EB9345C5344597BC94A864EDD38EE1}

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in Experience Cloud-oplossingen:

| Oplossing | Beschrijving |
|--- |--- |
| Cloud-publiek beleven | Maak, beheer en deel publiek native met behulp van de interface [Audience Library](../audience-library/audience-library.md) . U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br>Voor suggesties over welk type publiek u wilt creëren zie: Ervaar [Cloud-publiek](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analyse | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment [publiceren aan de Wolk](../audience-library/audience-library.md)van de Ervaring. Als u het segment publiceert, wordt dit op de pagina [Soorten publiek](../audience-library/audience-library.md) weergegeven. Het publiek is ook beschikbaar als doelgroep voor een campagneervaring die wordt geleverd door Adobe Target en in Audience Manager. Zodra een publiek van Analytics wordt gedeeld, en voor gebruik in een actieve campagne wordt geselecteerd, worden alle bezoekersprofielen die aan de criteria van de segmentdefinitie voor de afgelopen 90 dagen voldeden verzonden naar het platform van de Diensten [!UICONTROL van het] Publiek van de Ervaring Cloud. De grens voor gedeeld publiek is verhoogd tot 75. Het publiek dat via Analytics naar de Experience Cloud wordt gedeeld, mag niet meer dan 20 miljoen unieke leden tellen. Vanwege caching is het bovendien 12 uur nodig voordat verwijderde rapportsuites in Analytics worden weergegeven in de Experience Cloud. |
| Mobiele services | Analyseer mobiel verkeer gebruikend de zonneburst visualisatie in het rapport van de Types [!UICONTROL van] Apparaat. |
| Doel | Met de [id-service](https://docs.adobe.com/content/help/en/id-service/using/home.html) verenigt u gebruikers-id&#39;s en gegevens in één actionabel profiel voor gebruik in verschillende oplossingen. Met het selectievakje [Publiceren naar de Experience Cloud](../audience-library/audience-library.md) tijdens het maken van segmenten in Adobe Analytics kan het segment beschikbaar zijn in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat in Analytics of de Manager van de Publiek wordt gecreeerd kan voor activiteiten in Doel worden gebruikt.  U kunt bijvoorbeeld campagneactiviteiten maken op basis van de omzettingswaarden voor Analytics en publiekssegmenten die zijn gemaakt in Analytics. |
| Auditiebeheer | Gedeeld publiek is beschikbaar in segmentatie van Audience Manager. Alle Experience Cloud-soorten zijn standaard beschikbaar in Audience Manager, die het volgende biedt:<ul><li>Ingebouwde automatisering betreffende hoe zij worden gedeeld en in oplossingswerkschema&#39;s verbruikt</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campagne | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-oplossingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-oplossingen die u gebruikt.</li></ul> |
| Media optimaliseren | Gebruik het publiek als doelen. |

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4 tot 8 uur voordat die informatie kan worden gebruikt in Target, Ad Cloud en Campagnestandaard.

## Meer hulp - vragen, begeleiding en gebruiksgevallen {#section_C7F151644D8A45F7B6FC54F58845635D}

| Help met | Resource |
|--- |--- |
| Kan publiek niet vinden? | Zorg ervoor dat u provisioned bent. Zie [Aan de slag - stel uw oplossingen in voor de kernservices](../core-services/core-services.md).<br>Klik [hier](https://www.adobe.com/go/audiences) om toegang te vragen tot profielen en soorten publiek (inrichtingsformulier voor integraties). |
| Gebruik hoofdletters | Voor meer begeleiding op welke oplossing te gebruiken, ga naar de Opties [van de Aanmaak van het](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html) publiek in de Kennisbank. |
| Forum | Het [Soortforum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) is een extra bron voor hulp bij het publiek. |

## Audio Library-interface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

Het [!DNL Experience Cloud] biedt een bibliotheek voor het maken en beheren van soorten publiek, met native, realtime publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL Personen]** > **[!UICONTROL Audience Library]**

![](assets/audience_library.png)

| Element | Beschrijving |
|--- |--- |
| Nieuw | [Een doelgroep maken](../audience-library/audience-library.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Bron | Identificeert waar het publiek is gemaakt.<ul><li>**Analyse:** Een segment dat is gemaakt in rapporten en analyses of ad-hocanalyses en vervolgens wordt [gepubliceerd naar de Experience Cloud](../audience-library/audience-library.md).</li><li>**Experience Cloud:** Een nieuw publiek [gemaakt in Experience Cloud Audiences](../audience-library/audience-library.md).</li><li>**Audience Manager:** Soorten publiek die Audience Manager hebben gemaakt, worden automatisch weergegeven in de Experience Cloud Audiences.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |
