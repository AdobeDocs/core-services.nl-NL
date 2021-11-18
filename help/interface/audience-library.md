---
solution: Experience Cloud
type: Documentation
title: 'Adobe Experience Cloud-publiek '
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
description: Leer hoe u de vertaling van bezoekersgegevens in publiekssegmentatie in de service Experience Cloud Audience beheert.
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 2%

---

# Experience Cloud-publiek {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Soorten publiek zijn verzamelingen bezoekers (een lijst met bezoekers-id&#39;s). Met de Audience Library kunt u de omzetting van bezoekersgegevens in publiekssegmentatie beheren. Als dusdanig, is het creëren van, en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten. U kunt het publiekssegment ook delen met producten en services in [!DNL Experience Cloud].

![Experience Cloud-publiek](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe in het dialoogvenster [!DNL Experience Cloud]
* [!DNL Analytics] segmenten gepubliceerd naar de [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Real-Time versus historisch publiek**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime doelwitten. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden om de vier uur geëvalueerd. De totale tijd om te verwerken en te delen neemt tot acht uur in beslag. Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Het publiek in real time wordt afkomstig uit het publiek van de Experience Cloud en geëvalueerd in echt - tijd.

## Hoe toepassingen publiek gebruiken {#concept_01EB9345C5344597BC94A864EDD38EE1}

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in Experience Cloud-toepassingen:

| Oplossing | Beschrijving |
|--- |--- |
| Experience Cloud publiek | Maak, beheer en deel publiek native met de opdracht [Auditiebibliotheek](audience-library.md) interface. U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br>Voor suggesties over welk type publiek u wilt creëren zie: [Experience Cloud publiek](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=en). |
| Analytics | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment aan Experience Cloud publiceren. Het publiceren van het segment toont het op het [!UICONTROL Audience Library] pagina in Experience Cloud. (Zie [Segmenten publiceren naar de Experience Cloud](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=en) in de Help bij Analytics voor meer informatie.) Het publiek is ook beschikbaar als doelgroep voor een campagneervaring die door Adobe Target en in de Audience Manager wordt opgeleverd. Nadat u een publiek van Adobe Analytics deelt, en het voor gebruik in een actieve campagne selecteert, worden de bezoekersprofielen die aan de criteria van de segmentdefinitie voor de afgelopen 90 dagen voldoen verzonden naar [!UICONTROL Audience Services]. De grens voor gedeeld publiek is verhoogd tot 75. Het publiek dat vanuit Analytics aan de Experience Cloud wordt gedeeld, mag niet meer dan 20 miljoen unieke leden tellen. Vanwege caching is het bovendien 12 uur nodig voordat de verwijdering in de Experience Cloud wordt weergegeven. |
| Mobiele services | Analyseer het mobiele verkeer met de zonneexplosie-visualisatie in de [!UICONTROL Device Types] verslag. |
| [!DNL Target] | De [ID-service](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=en) Hiermee verenigt u gebruikers-id&#39;s en gegevens in één actiefprofiel voor gebruik in verschillende toepassingen. De [Publiceren naar de Experience Cloud](audience-library.md) Schakel het selectievakje tijdens het maken van segmenten in Adobe Analytics in om het segment beschikbaar te maken in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat in Analytics of Audience Manager wordt gecreeerd kan voor activiteiten in worden gebruikt [!DNL Target]. U kunt bijvoorbeeld campagneactiviteiten maken op basis van [!DNL Analytics] conversiemetriek en publiekssegmenten gemaakt in [!DNL Analytics]. |
| Audience Manager | Gedeeld publiek is beschikbaar in segmentatie van de Audience Manager. Alle Experience Cloud-soorten zijn in de Audience Manager verkrijgbaar, met:<ul><li>Ingebouwde automatisering voor de manier waarop ze worden gedeeld en verbruikt in workflows van toepassingen</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campaign | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-toepassingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-toepassingen die u gebruikt.</li></ul> |
| Advertising Cloud | Gebruik het publiek als doelen. |

{style=&quot;table-layout:auto&quot;}

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4-8 uur voordat die informatie kan worden gebruikt in [!DNL Target], Ad Cloud en Campaign Standard.

## Meer hulp - vragen, begeleiding en gebruiksgevallen {#section_C7F151644D8A45F7B6FC54F58845635D}

| Help met | Resource |
|--- |--- |
| Kan publiek niet vinden? | Zorg ervoor dat u provisioned bent. Zie [Aan de slag - uw toepassingen inschakelen voor kernservices](core-services.md).<br>Ga [hier](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES) toegang tot profielen en soorten publiek aanvragen (inrichtingsformulier voor integraties). |
| Gebruiksscenario’s | Ga voor meer informatie over de toepassing die u wilt gebruiken naar [Opties voor het maken van publiek](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=en) in de Kennisbank. |
| Forum | De [Publiek forum](https://experienceleaguecommunities.adobe.com/t5/Adobe-Experience-Cloud-Audiences/ct-p/experience-cloud-audiences-community) is een andere bron voor hulp bij het publiek. |

{style=&quot;table-layout:auto&quot;}

## Audio Library-interface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

De [!DNL Experience Cloud] biedt een bibliotheek voor het maken en beheren van doelgroepen, met native, realtime publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![publiek toevoegen in Auditiebibliotheek](assets/audience_library.png)

| Element | Beschrijving |
|--- |--- |
| Nieuw | [Een doelgroep maken](audience-library.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Bron | Identificeert waar het publiek is gemaakt.<ul><li>**Analyse:** Een segment gemaakt in Adobe Analytics, daarna [gepubliceerd aan de Experience Cloud](audience-library.md).</li><li>**Experience Cloud:** Een nieuw publiek [gemaakt in publiek Experience Cloud](audience-library.md).</li><li>**Audience Manager:** Het publiek creeerde Audience Manager toont automatisch in het Publiek van de Experience Cloud.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |

{style=&quot;table-layout:auto&quot;}
