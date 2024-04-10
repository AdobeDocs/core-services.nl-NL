---
description: Veelgestelde vragen over [!DNL Customer Attributes] in Adobe Experience Cloud, voor Adobe Analytics en Adobe Target.
solution: Experience Cloud
title: Veelgestelde vragen over [!DNL Customer Attributes]
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 1%

---

# Veelgestelde vragen over [!DNL Customer Attributes]

Veelgestelde vragen en aanbevolen procedures voor [!DNL Customer Attributes] in Adobe Analytics en Adobe Target.

## Best practices en beperkingen {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Richtlijnen en beperkingen bij gebruik [!DNL Customer Attributes].

| Probleem | Beschrijving |
|--- |--- |
| [!UICONTROL Customer attribute] abonnementsbeperkingen | Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er meer kenmerken beschikbaar zijn. Misschien ziet u een [!UICONTROL Attribute Subscription Max] fout tijdens deze vertraging. |
| Meerdere aanmeldingen op hetzelfde apparaat | Wanneer u [!DNL Customer Attributes] om klantprofielen in een gegevensbron te uploaden, adviseert de Adobe tegen gebruikers die apparaten delen (die, zelfde Experience Cloud ID) betekent. De Experience Cloud-id (ECID) blijft bestaan op het apparaat. Door apparaten te delen kan de ECID meerdere gebruikers aan dezelfde ECID koppelen, wat onverwachte resultaten tot gevolg heeft [!DNL Target]. **Opmerking:** Voor mobiele apparaten is de ECID blijvend nadat de mobiele toepassing is geïnstalleerd. Installeer de toepassing opnieuw om een nieuwe ECID te genereren. Voor het Web, wordt een nieuwe ECID geproduceerd nadat het browser koekje wordt ontruimd. |
| Maximale uploadfrequentie per dag | Adobe raadt u aan de update uit te voeren [!DNL Customer Attributes] slechts eenmaal per dag. U moet ten minste 24 uur wachten om een ander bestand met klantprofielgegevens te uploaden voor dezelfde set profielen. |
| Aangepaste analyse-id (`s.visitorID`) | Een klant-id instellen met `s.visitorID` is een methode om gebruikers in Analytics te identificeren. Integraties waarin [!DNL Analytics] gegevens worden geëxporteerd of geïmporteerd met de ID-service functioneren niet wanneer een bezoeker wordt geïdentificeerd met `s.visitorID.`<br>Dit omvat, maar is niet beperkt tot, het gedeelde publiek, [!DNL Analytics] voor Adobe Target (A4T), en [!DNL Customer Attributes].<br>Voor deze integraties wordt het instellen van een aangepaste Analytics-id niet ondersteund. |
| Tekenlengtebeperkingen in [!DNL Analytics] | Wanneer u een [!DNL Analytics] abonnement, de veldlengten voor de geüploade bestanden worden ingekort tot 255. |

{style="table-layout:auto"}

## FAQ over [!DNL Customer Attributes] {#section_E47866EEA83348E09FE43CEC5E44C461}

| Vraag | Antwoord |
|--- |--- |
| Kan ik meldingen ontvangen over de uploadstatus voor [!DNL Customer Attributes]? | Ja. |
| Wat moet ik doen om mee te beginnen? [!DNL Customer Attributes]? | <ol><li>Ontvang provisioned. Als u een klant van de Analyse bent, voorziet de Adobe u voor [!DNL Customer Attributes]. Als u alleen Adobe Target gebruikt en geen Analytics hebt, kunt u de levering voor de kernservices aanvragen door contact op te nemen met de klantenservice.</li> <li>Heb een gesprek met uw team van CRM. Ontdek welk soort klantgegevens beschikbaar zijn die u in Analytics en door Experience Cloud wilt gebruiken.</li><li>De kernservices implementeren. Zie [Uw toepassingen inschakelen voor kernservices](core-services.md) voor stappen over hoe te om uw implementatie te moderniseren. (Zie de sectie over het synchroniseren van klant-id&#39;s voor belangrijke informatie.)</li></ol> **Opmerking:** De FAQ van een beheerder voor het uitvoeren van de kerndiensten is beschikbaar [hier](faq.md). |
| Hoeveel [!DNL Customer Attributes] Mag ik gebruiken? | U kunt honderden `.csv` kolommen aan de dienst van Attributen van de Klant. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten (per rapportsuite), afhankelijk van de toepassingen die u hebt:  <ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200</li><li>Adobe Target-standaard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Is migratie naar de Experience Cloud-id-service vereist? | De migratie is afhankelijk van de toepassingen die u gebruikt. <ul><li>Adobe Analytics: sterk aanbevolen </li><li>Adobe Target: vereist. </li></ul><br>Het gebruiken van de dienst van identiteitskaart van het Experience Cloud laat de recentste functionaliteit van het Experience Cloud, met inbegrip van publiek in real time, de modernisering van Adobe Target, de integratie van Analytics, en videokopartmaattracking toe. <br> Zie voor meer informatie [Uw toepassingen inschakelen voor kernservices](core-services.md). <br>**Opmerking:** De [Experience Cloud-id-service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=en) is de gemoderniseerde uitvoering van wat vroeger bekend staat als _Analyse van bezoeker-id-service._ |
| Hoe verhoudt de kenmerkfunctionaliteit van de Klant zich tot Adobe Audience Manager? | Hoewel de Audience Manager gegevens kan ontvangen om publieksidentificatie uit te voeren, kan het geen analysefunctionaliteit uitvoeren die attributen aan historische gedragsgegevens bindt. Het biedt ook niet de rapportage-, analyse- en segmentatiemogelijkheden die beschikbaar zijn in Adobe Analytics. [!UICONTROL People] laat rijke gegevens van over toepassingen toe om samen worden gebonden en met één enkele identiteitskaart voor gebruik over Experience Cloud worden geassocieerd. <br>In Adobe Target: [!DNL Customer Attributes] verschijnen als individuele attributen die met andere regels kunnen worden gecombineerd om publiek te bouwen. Voor de [!UICONTROL People] de dienst is volledig publiek dat niet kan worden gewijzigd. |
| **(Alleen analyse)** Hoe verschilt deze functionaliteit van wat in de premie van Analytics wordt verstrekt? | In het verleden hebben klanten die klantkenmerkgegevens willen combineren met analysegegevens, voor deze functionaliteit sterk vertrouwd op de Data Workbench-tool. [!DNL Customer Attributes] deze functionaliteit toegankelijk maken voor een groter publiek door [!DNL Customer Attributes] als afmetingen en metriek in rapporten &amp; analyses, Ad Hoc Analysis, en rapportaannemer. Klanten met analysestandaard hebben toegang tot [!DNL Customer Attributes], maar met beperkte mogelijkheden. De volledige functionaliteit is beschikbaar voor klanten van de Analytics Premium. |
| **(Alleen Adobe Target)** Kan ik gegevens vooraf laden of uploaden voor klanten die Adobe Target nog nooit heeft gezien? | Ja. Wanneer de bezoeker zijn eerste verzoek aan Adobe Target indient, haalt het systeem de bestaande informatie-Adobe over hen van [!DNL Customer Attributes] en gebruiken die gegevens voor het richten. **Opmerking:**  Het ophalen van deze gegevens kan tot 20 minuten duren na de eerste interactie van de bezoeker met Adobe Target. |
| **(Alleen Adobe Target)** Kan ik een superpubliek creëren door de gegevens van Attributen van de Klant met gedeelde publieksgegevens te combineren? | Nee. Gegevens voor een gedeeld publiek zijn voltooid. |
| **(alleen Adobe Target)** Hoe doet het [!DNL Customer Attributes] functionaliteit vergeleken met Adobe Target bulkprofiel-API? | Met de API voor bulkprofielen kunnen Adobe Target-profielen rechtstreeks via de API worden bijgewerkt, voor een afzonderlijk profiel of in bulk. De capaciteit is gelijkaardig aan [!DNL Customer Attributes], met de volgende belangrijke verschillen:<ul><li>De profiel-API is een REST API-aanroep en [!DNL Customer Attributes] gebruikt FTP.</li><li>Adobe Target-profiel-API verzendt alleen gegevens naar Adobe Target in plaats van naar het hele Experience Cloud.</li><li>[!DNL Customer Attributes] biedt een eenvoudige interface voor het maken en beheren van deze externe gegevens.</li></ul> |
| **(alleen Adobe Target)** Hiermee worden gegevens geüpload van [!DNL Customer Attributes] of Adobe Target de levensduur van het profiel van de Adobe Target-bezoeker verlengt? | Ja. Zie [Levensduur bezoekersprofiel](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=en) in Adobe Target Help. |
| **(alleen Adobe Target)** Kan ik me richten op de gegevens die zijn geüpload in [!DNL Customer Attributes] onmiddellijk nadat de bezoeker door de klant-id wordt geïdentificeerd? | Ja. Op de serveroproep aan Adobe Target, die de id van een derde partij mbox bevat, zijn alle gegevens van Kenmerk van klant beschikbaar. |
| **(alleen Adobe Target)** Wat doet de **[!UICONTROL Sync Status]** de kolom vertegenwoordigt voor dossiers die in de bron van Attributen van de Klant worden geupload? | Het aantal records dat door Adobe Target is gepubliceerd en gesynchroniseerd, kan worden weergegeven door het pictogram Synchronisatiestatus te selecteren op basis van een specifiek kenmerkbestand. `Sync %` is een real-time metrisch die het percentage van profielen specificeert die in Adobe Target zijn gesynchroniseerd.<br> **Opmerking:** Het kan 24 uur duren voordat kenmerken worden gesynchroniseerd met Adobe Target. |
| Wat vertegenwoordigen de gegevens voor het uploaden van bestanden in [!DNL Customer Attributes] Bron? | U kunt de status controleren van kenmerken waarnaar geüpload wordt [!DNL Customer Attributes] met behulp van de volgende metingen: <ul><li>Records: Aantal records in het kenmerkbestand.</li><li>**Nieuwe records:** Aantal nieuwe records in het kenmerkbestand.</li> <li>**Bijgewerkte records:** Aantal records in dat bestaat in [!DNL Customer Attributes] met bijgewerkte waarden in het bestand.</li><li>**Alle gegevens (records):** Totaal aantal records geüpload naar [!DNL Customer Attributes].</li></ul> |

{style="table-layout:auto"}