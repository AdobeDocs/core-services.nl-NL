---
title: "[!DNL Audience Library]"
description: Leer hoe u het vertalen van bezoekersgegevens naar publiekssegmentatie in Experience Cloud beheert [!DNL Audience Library].
solution: Experience Cloud
type: Documentation
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: 064f3c981b921fd5aec9b252b839d8b7f59b3dee
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 2%

---

# Experience Cloud publiek {#topic_679810123CAA4E0CA4FA3417FB0100C7}

De [!DNL Audience Library] geeft het publiek in Experience Cloud weer. Soorten publiek zijn verzamelingen bezoekers (een lijst met [!DNL Experience Cloud] ID&#39;s). U kunt de vertaling van bezoekersgegevens in publiekssegmentatie beheren. Als zodanig lijkt het maken en beheren van soorten publiek op het maken en gebruiken van segmenten. U kunt het publiekssegment ook delen met producten en services in [!DNL Experience Cloud].

![Experience Cloud publiek](assets/audiences.png)

De soorten publiek kunnen van diverse bronnen tot stand worden gebracht of worden afgeleid, zoals:

* Nieuwe in het dialoogvenster [!DNL Experience Cloud]
* [!DNL Analytics] segmenten gepubliceerd naar de [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Real-Time versus historisch publiek**

Alle doelgroepen, ongeacht waar ze vandaan komen, zijn toegankelijk voor gebruiksgevallen in realtime. Het publiek dat wordt gedeeld van Analytics naar Audience Manager, is echter niet toegankelijk voor realtime doelwitten. Het systeem evalueert het publiek op twee manieren:

* Historische doelgroepen van Analytics worden om de vier uur geëvalueerd. De totale tijd om te verwerken en te delen duurt tot acht uur. Historische doelgroepen omvatten altijd terugkeerbezoekers.
* Het publiek in real time wordt teruggebracht tot publiek van het Experience Cloud en in echt - tijd geëvalueerd.

## Hoe toepassingen publiek gebruiken {#concept_01EB9345C5344597BC94A864EDD38EE1}

In de volgende tabel wordt beschreven hoe publiek wordt gebruikt in toepassingen voor Experiencen Cloud:

| Oplossing | Beschrijving |
|--- |--- |
| Experience Cloud-doelgroepen | Eigen gebruikers maken, beheren en delen met [[!DNL Audience Library]](audience-library.md). U kunt:<ul><li>Real-time soorten publiek gebruiken met onbewerkte analysekenmerken</li><li>Combineer publiek om samengestelde degenen tot stand te brengen, verbindend real time en historische gegevens</li><li>Zie grafische weergaven van geschatte doelgrootte</li></ul><br>Voor suggesties over welk type publiek u wilt creëren zie [Opties voor het maken van publiek](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=en). |
| Analytics | In segmentatie, kunt u een segment bouwen, het met een rapportreeks combineren, en dan het segment aan Experience Cloud publiceren. Het publiceren van het segment toont het op het [!DNL Audience Library] pagina in Experience Cloud. (Zie [Segmenten publiceren naar Experience Cloud](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=en) in [!DNL Analytics] voor meer informatie.) Het publiek is ook beschikbaar als doelgroep voor een campagneervaring van [!DNL Adobe Target], en in [!DNL Audience Manager]. Nadat u een publiek hebt gedeeld vanuit [!DNL Adobe Analytics]en selecteert u deze voor gebruik in een actieve campagne. De bezoekersprofielen die de afgelopen 90 dagen aan de criteria voor segmentdefinitie voldoen, worden naar [!UICONTROL Audience Services]. De grens voor gedeeld publiek is verhoogd tot 75. Soorten publiek dat vanuit [!DNL Analytics] mag niet meer dan 20 miljoen unieke leden bedragen. Vanwege caching is het bovendien 12 uur nodig voordat de verwijdering in het Experience Cloud wordt weergegeven. |
| Mobiele services | Analyseer het mobiele verkeer met de zonneexplosie-visualisatie in de [!UICONTROL Device Types] verslag. |
| [!DNL Target] | De [ID-service](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=en) Hiermee verenigt u gebruikers-id&#39;s en gegevens in één actiefprofiel voor gebruik in verschillende toepassingen. De [Publiceren naar Experience Cloud](audience-library.md) Schakel het selectievakje tijdens het maken van segmenten in Adobe Analytics in om het segment beschikbaar te maken in de aangepaste publieksbibliotheek van Adobe Target. Een segment dat is gemaakt in [!DNL Analytics] of [!DNL Audience Manager] kan worden gebruikt voor activiteiten in [!DNL Target]. U kunt bijvoorbeeld campagneactiviteiten maken op basis van [!DNL Analytics] conversiemetriek en publiekssegmenten gemaakt in [!DNL Analytics]. |
| [!DNL Audience Manager] | Gedeeld publiek is beschikbaar in [!DNL Audience Manager] segmentatie. Alle soorten publiek in het Experience Cloud zijn standaard beschikbaar in [!DNL Audience Manager], die voorziet in:<ul><li>Ingebouwde automatisering voor de manier waarop ze worden gedeeld en verbruikt in workflows van toepassingen</li><li>Offsite doelen</li><li>Modellering van look-alike</li></ul> |
| Campaign | <ul><li>Importeer een gedeeld publiek van verschillende Adobe Experience Cloud-toepassingen naar Adobe Campaign.</li><li>Lijst met ontvangers exporteren in de vorm van een gedeeld publiek. Deze gedeelde doelgroepen kunnen worden gebruikt in de verschillende Adobe Experience Cloud-toepassingen die u gebruikt.</li></ul> |
| Advertising Cloud | Gebruik het publiek als doelen. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Wanneer een bezoeker in aanmerking komt voor het publiek dat wordt gedeeld door Analytics, is er een vertraging van 4-8 uur voordat die informatie kan worden gebruikt in [!DNL Target], Ad Cloud en Campaign Standard.

## Meer hulp - vragen, begeleiding en gebruiksgevallen {#section_C7F151644D8A45F7B6FC54F58845635D}

| Help met | Bron |
|--- |--- |
| Kan publiek niet vinden? | Zorg ervoor dat u provisioned bent. Zie [Aan de slag - uw toepassingen inschakelen voor kernservices](core-services.md).<br>Ga [hier](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES) toegang tot profielen en soorten publiek aanvragen (inrichtingsformulier voor integraties). |
| Forum | De [Publiek forum](https://experienceleaguecommunities.adobe.com/t5/Adobe-Experience-Cloud-Audiences/ct-p/experience-cloud-audiences-community) is een andere bron om hulp te krijgen bij het publiek. |

{style="table-layout:auto"}

## Audio Library-interface-elementen {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

De [!DNL Experience Cloud] biedt een bibliotheek voor het maken en beheren van doelgroepen, met native, realtime publieksidentificatie.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![publiek toevoegen in Auditiebibliotheek](assets/audience_library.png)

| Element | Beschrijving |
|--- |--- |
| Nieuw | [Een publiek maken](audience-library.md). |
| Titel en beschrijving | Een kolomkop die het publiek identificeert en beschrijft. |
| Auteur | De persoon die het publiekssegment creeerde. |
| Bron | Identificeert waar het publiek is gemaakt.<ul><li>**Analyse:** Een segment gemaakt in Adobe Analytics, daarna [gepubliceerd naar Experience Cloud](audience-library.md).</li><li>**Experience Cloud:** Een nieuw publiek [gemaakt in publiek Experience Cloud](audience-library.md).</li><li>**Audience Manager:** Het publiek creeerde Audience Manager toont automatisch in het Publiek van het Experience Cloud.</li></ul> |
| Huidige grootte | De huidige publieksgrootte. |
| Actief | De actieve status van het segment. |

{style="table-layout:auto"}
