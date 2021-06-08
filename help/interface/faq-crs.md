---
description: Veelgestelde vragen over klantkenmerken in Adobe Experience Cloud, voor Adobe Analytics en Adobe Target.
keywords: Klantkenmerken
solution: Experience Cloud
title: 'Antwoorden krijgen op veelgestelde vragen over Customer Attributes '
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
feature: Klantkenmerken
topic: Beheer
role: Administrator
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: eef7326f9f04f68eefb60b5d9fd4cc91cbe52119
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 1%

---

# Veelgestelde vragen over [!UICONTROL Customer Attributes]

Veelgestelde vragen en aanbevolen procedures voor [!UICONTROL Customer Attributes] in Adobe Analytics en Adobe Target.

## Best practices en beperkingen {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Richtlijnen en beperkingen bij gebruik van [!UICONTROL Customer Attributes].

| Probleem | Beschrijving |
|--- |--- |
| [!UICONTROL Customer attribute] abonnementsbeperkingen | Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er meer kenmerken beschikbaar zijn. Tijdens deze vertraging kan een fout [!UICONTROL Attribute Subscription Max] worden weergegeven. |
| Meerdere aanmeldingen op hetzelfde apparaat | Als u [!UICONTROL Customer Attributes] gebruikt om klantprofielen te uploaden naar een gegevensbron, raadt Adobe gebruikers aan apparaten niet te delen (wat hetzelfde betekent, dezelfde Experience Cloud-id). De Experience Cloud-id (ECID) blijft bestaan op het apparaat. Door apparaten te delen kan de ECID meerdere gebruikers aan dezelfde ECID koppelen, wat onverwachte resultaten tot gevolg heeft in [!DNL Target]. **Opmerking:** Voor mobiele apparaten is de ECID blijvend nadat de mobiele toepassing is geïnstalleerd. Installeer de toepassing opnieuw om een nieuwe ECID te genereren. Voor het Web, wordt een nieuwe ECID geproduceerd nadat het browser koekje wordt ontruimd. |
| Maximale uploadfrequentie per dag | Adobe raadt u aan de klantkenmerken slechts eenmaal per dag bij te werken. U moet ten minste 24 uur wachten om een ander bestand met klantprofielgegevens te uploaden voor dezelfde set profielen. |
| Custom Analytics ID (`s.visitorID`) | Het instellen van een klant-id met `s.visitorID` is een methode om gebruikers in Analytics te identificeren. Integraties waarin [!DNL Analytics]-gegevens worden geëxporteerd of geïmporteerd met behulp van de ID-service functioneren echter niet wanneer een bezoeker wordt geïdentificeerd met behulp van `s.visitorID.`<br>Dit omvat, maar is niet beperkt tot, gedeelde soorten publiek, [!DNL Analytics] voor Adobe Target (A4T) en [!UICONTROL Customer Attributes].<br>Voor deze integraties wordt het instellen van een aangepaste Analytics-id niet ondersteund. |
| Tekenlengtebeperkingen in [!DNL Analytics] | Wanneer u een [!DNL Analytics]-abonnement maakt, wordt de veldlengte voor de geüploade bestanden afgebroken tot 255. |

## Veelgestelde vragen over klantkenmerken {#section_E47866EEA83348E09FE43CEC5E44C461}

| Vraag | Antwoord |
|--- |--- |
| Kan ik meldingen ontvangen over de status van uploaden naar Customer Attributes? | Ja. |
| Wat moet ik doen om aan de slag te gaan met Customer Attributes? | <ol><li>Ontvang provisioned. Als u een klant van de Analyse bent, voorziet Adobe u voor de Attributen van de Klant. Als u alleen Adobe Target gebruikt en geen Analytics hebt, kunt u de levering voor de kernservices aanvragen door contact op te nemen met de klantenservice.</li> <li>Heb een gesprek met uw team van CRM. Ontdek welk type van klantengegevens beschikbaar is dat u in Analytics en door de Experience Cloud wilt gebruiken.</li><li>De kernservices implementeren. Zie [Het toelaten van uw oplossingen voor kerndiensten](core-services.md) voor stappen op hoe te om uw implementatie te moderniseren. (Zie de sectie over het synchroniseren van klant-id&#39;s voor belangrijke informatie.)</li></ol> **Nota:** Veelgestelde vragen van een beheerder voor het uitvoeren van de kerndiensten is beschikbaar  [hier](faq.md). |
| Hoeveel Kenmerken van de Klant mag ik gebruiken? | U kunt honderden `.csv` kolommen aan de dienst van Attributen van de Klant uploaden. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten (per rapportsuite), afhankelijk van de oplossingen die u hebt:  <ul><li>Stichting: 0</li><li>Selecteren: 1</li><li>Primair: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200</li><li>Adobe Target-standaard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Is migratie naar de Experience Cloud ID-service vereist? | Migratie is afhankelijk van de oplossingen die u gebruikt. <ul><li>Adobe Analytics: Sterk aanbevolen </li><li>Adobe Target: Vereist. </li></ul><br>Het gebruiken van de dienst van identiteitskaart van de Experience Cloud laat de recentste functionaliteit van de Experience Cloud, met inbegrip van publiek in real time, de modernisering van Adobe Target, de integratie van Analytics, en videohartslag het volgen toe. <br> Voor meer details, zie  [Enable uw oplossingen voor de kerndiensten](core-services.md). <br>**Opmerking:** De  [Experience Cloud ID-](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=en) service is de gemoderniseerde implementatie van wat voorheen bekend stond als  _Analytics bezoeker ID-service._ |
| Hoe verhoudt de kenmerkfunctionaliteit van de Klant zich tot Adobe Audience Manager? | Hoewel de Audience Manager gegevens kan ontvangen om publieksidentificatie uit te voeren, kan het geen analysefunctionaliteit uitvoeren die attributen aan historische gedragsgegevens bindt. Het biedt ook niet de rapportage-, analyse- en segmentatiemogelijkheden die beschikbaar zijn in Adobe Analytics. [!UICONTROL People] laat rijke gegevens van over oplossingen toe om samen en geassocieerd met één enkele identiteitskaart voor gebruik over de Experience Cloud worden gebonden. <br>In Adobe Target worden klantkenmerken weergegeven als afzonderlijke kenmerken die kunnen worden gecombineerd met andere regels om een publiek te maken. Het publiek dat aan de [!UICONTROL People] dienst wordt gedeeld is volledig publiek dat niet kan worden gewijzigd. |
| **(Alleen Analytics)** Hoe verschilt deze functionaliteit van wat er in de premie Analytics wordt aangeboden? | In het verleden hebben klanten die klantkenmerkgegevens willen combineren met analysegegevens, voor deze functionaliteit sterk vertrouwd op de Data Workbench-tool. [!UICONTROL Customer Attributes] stelt deze functionaliteit aan een groter publiek bloot door de Attributen van de Klant als afmetingen en metriek in rapporten &amp; analytics, Ad Hoc Analysis, en rapportaannemer te verstrekken. Klanten met standaardanalysemogelijkheden hebben toegang tot klantkenmerken, maar met beperkte mogelijkheden. De volledige functionaliteit is beschikbaar voor klanten van de Analytics Premium. |
| **(Alleen Adobe Target)** Kan ik gegevens vooraf laden of uploaden voor klanten die Adobe Target nog nooit heeft gezien? | Ja. Wanneer de bezoeker zijn eerste verzoek aan Adobe Target indient, haalt het systeem de bestaande informatie die Adobe over hen van de Attributen van de Klant heeft en gebruikt die gegevens voor het richten. **Opmerking:**  het ophalen van deze gegevens kan tot 20 minuten duren na de eerste interactie van de bezoeker met Adobe Target. |
| **(Alleen Adobe Target)** Kan ik een superpubliek maken door klantkenmerkgegevens te combineren met gedeelde publieksgegevens? | Nee. Gegevens voor een gedeeld publiek zijn voltooid. |
| **(Alleen Adobe Target)** Hoe verhoudt de  [!UICONTROL Customer Attributes] functionaliteit zich tot de Adobe Target-API voor bulkprofielen? | Met de API voor bulkprofielen kunnen Adobe Target-profielen rechtstreeks via de API worden bijgewerkt, voor een afzonderlijk profiel of in bulk. De capaciteit is gelijkaardig aan de Attributen van de Klant, met de volgende belangrijkste verschillen:<ul><li>De profiel-API is een REST API-aanroep en klantkenmerken gebruiken FTP.</li><li>Adobe Target-profiel-API verzendt alleen gegevens naar Adobe Target in plaats van naar de hele Experience Cloud.</li><li>Klantkenmerken bieden een eenvoudige interface voor het maken en beheren van deze externe gegevens.</li></ul> |
| **(Alleen Adobe Target)** Verlengt het uploaden van gegevens van Customer Attributes naar Adobe Target de levensduur van het profiel van de Adobe Target-bezoeker? | Ja. Zie [Levensduur bezoekersprofiel](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=en) in Adobe Target Help. |
| **(Alleen Adobe Target)** Kan ik me richten op de gegevens die direct nadat de bezoeker door de klant-id is geïdentificeerd in Customer Attributes zijn geüpload? | Ja. Op de serveroproep aan Adobe Target, die de id van een derde partij mbox bevat, zijn alle gegevens van Kenmerk van klant beschikbaar. |
| **(Alleen Adobe Target)** Wat vertegenwoordigt de  **[!UICONTROL Sync Status]** kolom voor bestanden die zijn geüpload in de kenmerkbron van de klant? | Het aantal records dat door Adobe Target is gepubliceerd en gesynchroniseerd, kan worden weergegeven door op het pictogram Synchronisatiestatus te klikken op een specifiek kenmerkbestand. `Sync %` is een real-time metrisch die het percentage van profielen specificeert die in Adobe Target zijn gesynchroniseerd.<br> **Opmerking:** het kan 24 uur duren voordat kenmerken worden gesynchroniseerd met Adobe Target. |
| Wat vertegenwoordigen de gegevens van het dossierupload in de Bron van Attributen van de Klant? | U kunt de status controleren van kenmerken die naar Klantkenmerken zijn geüpload met behulp van de volgende metingen: <ul><li>Records:  Aantal records in het kenmerkbestand.</li><li>**Nieuwe records:** aantal nieuwe records in het kenmerkenbestand.</li> <li>**Bijgewerkte records:** Aantal records in dat bestaat in Kenmerken van klant met bijgewerkte waarden in het bestand.</li><li>**Alle gegevens (records):** Totaal aantal records dat is geüpload naar Customer Attributes.</li></ul> |
