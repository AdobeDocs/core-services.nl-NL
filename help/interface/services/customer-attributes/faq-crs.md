---
description: Veelgestelde vragen over  [!DNL customer attributes]  in Adobe Experience Cloud, voor Adobe Analytics en Adobe Target.
solution: Experience Cloud
title: Veelgestelde vragen over  [!DNL customer attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 0%

---

# Veelgestelde vragen over [!DNL customer attributes]

Veelgestelde vragen en aanbevolen procedures voor [!DNL customer attributes] in Adobe Analytics en Adobe Target.

## Best practices en beperkingen {#best_practices}

Richtlijnen en beperkingen bij gebruik van [!DNL customer attributes] .

| Probleem | Beschrijving |
|--- |--- |
| [!UICONTROL customer attribute] abonnementsbeperkingen | Wanneer u een upgrade uitvoert naar de Analytics Premium, duurt het 24 uur voordat er meer kenmerken beschikbaar zijn. Tijdens deze vertraging wordt mogelijk een [!UICONTROL attribute Subscription Max] -fout weergegeven. |
| Meerdere aanmeldingen op hetzelfde apparaat | Als u [!DNL customer attributes] gebruikt om klantprofielen te uploaden naar een gegevensbron, raadt Adobe gebruikers aan apparaten niet te delen (wat hetzelfde betekent, dezelfde Experience Cloud-id). De Experience Cloud-id (ECID) blijft bestaan op het apparaat. Door apparaten te delen kan de ECID meerdere gebruikers aan dezelfde ECID koppelen, wat onverwachte resultaten tot gevolg heeft in [!DNL Target] . **Nota:** voor Mobiele, ECID is permanent nadat Mobiele app wordt geïnstalleerd. Installeer de toepassing opnieuw om een nieuwe ECID te genereren. Voor het Web, wordt een nieuwe ECID geproduceerd nadat het browser koekje wordt ontruimd. |
| Maximale uploadfrequentie per dag | Adobe raadt u aan [!DNL customer attributes] slechts eenmaal per dag bij te werken. U moet ten minste 24 uur wachten om een ander bestand met klantprofielgegevens te uploaden voor dezelfde set profielen. |
| Custom Analytics ID (`s.visitorID`) | Het instellen van een klant-id met `s.visitorID` is een manier om gebruikers in Adobe Analytics te identificeren. Integraties waarin [!DNL Analytics] -gegevens worden geëxporteerd of geïmporteerd met behulp van de ID-service functioneren echter niet wanneer een bezoeker wordt geïdentificeerd met `s.visitorID.`<br> Dit omvat, maar is niet beperkt tot, gedeelde soorten publiek, [!DNL Analytics] voor Adobe Target (A4T) en [!DNL customer attributes] .<br> voor deze integraties, wordt het plaatsen van een identiteitskaart van de douaneAnalytics niet gesteund. |
| Tekenlengtebeperkingen in [!DNL Analytics] | Wanneer u een [!DNL Analytics] -abonnement maakt, wordt de veldlengte voor de geüploade bestanden afgebroken tot 255. |

{style="table-layout:auto"}

## Veelgestelde vragen over [!DNL customer attributes] {#section_E47866EEA83348E09FE43CEC5E44C461}

| Vraag | Antwoord |
|--- |--- |
| Kan ik meldingen ontvangen over de uploadstatus voor [!DNL customer attributes]? | Ja. |
| Wat moet ik doen om aan de slag te gaan met [!DNL customer attributes]? | <ol><li>Ontvang provisioned. Als u een Adobe Analytics-klant bent, wordt u door Adobe geleverd voor [!DNL customer attributes] . Als u alleen Adobe Target gebruikt en geen Analytics hebt, vraagt u om provisioning voor kernservices door contact op te nemen met de klantenservice.</li> <li>Heb een gesprek met uw team van CRM. Ontdek welk soort klantgegevens beschikbaar zijn in Analytics en in Experience Cloud.</li><li>De kernservices implementeren.</li></ol> |
| Hoeveel [!DNL customer attributes] mag ik gebruiken? | U kunt honderden `.csv` kolommen uploaden naar de klantenkenmerkservice. Wanneer u echter abonnementen configureert en kenmerken selecteert, gelden de volgende limieten (per rapportsuite), afhankelijk van de toepassingen die u hebt:  <ul><li>Stichting: 0</li><li>Selecteren: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standaard: 3 totaal</li><li>Premium: 200</li><li>Adobe Target-standaard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Is migratie naar de Experience Cloud ID Service vereist? | De migratie is afhankelijk van de toepassingen die u gebruikt. <ul><li>Adobe Analytics: sterk aanbevolen </li><li>Adobe Target: vereist. </li></ul><br> Gebruikend de dienst van identiteitskaart van Experience Cloud laat de recentste functionaliteit van Experience Cloud, met inbegrip van publiek in real time, de modernisering van Adobe Target, de integratie van Analytics, en videohartslag het volgen toe. |
| Hoe heeft de functionaliteit van klantkenmerken betrekking op Adobe Audience Manager? | Hoewel Audience Manager gegevens kan ontvangen om publieksidentificatie uit te voeren, kan het geen analysefunctionaliteit uitvoeren die attributen aan historische gedragsgegevens bindt. Het biedt ook niet de rapportage-, analyse- en segmentatiemogelijkheden die beschikbaar zijn in Adobe Analytics. In [!UICONTROL Customer Attributes] kunnen rijke gegevens van verschillende toepassingen aan één id worden gekoppeld voor gebruik in Experience Cloud. <br> in Adobe Target, [!DNL customer attributes] verschijnen als individuele attributen die met andere regels kunnen worden gecombineerd om publiek te bouwen. Het publiek dat wordt gedeeld met de [!UICONTROL People] -service is een volledig publiek dat niet kan worden gewijzigd. |
| **(Adobe Analytics slechts)** hoe is deze functionaliteit verschillend van wat in de premie van Analytics wordt verstrekt? | In het verleden hebben klanten die in het combineren van klantkenmerkgegevens met Analytische gegevens geïnteresseerd zijn, voor deze functionaliteit sterk vertrouwd op het Data Workbench-hulpmiddel. [!DNL customer attributes] stelt deze functionaliteit beschikbaar voor een groter publiek door [!DNL customer attributes] op te geven als afmetingen en metriek in Report Builder. Klanten met Analytics Standard hebben toegang tot [!DNL customer attributes] , maar met beperkte mogelijkheden. De volledige functionaliteit is beschikbaar voor klanten van de Analytics Premium. |
| **(Alleen Adobe Target)** Kan ik gegevens voor klanten die Adobe Target nog nooit heeft gezien, vooraf laden of uploaden? | Ja. Wanneer de bezoeker voor het eerst een verzoek indient bij Adobe Target, haalt het systeem de bestaande informatie op waarover Adobe beschikt van [!DNL customer attributes] en gebruikt het die gegevens voor het richten. **Nota:** het terugwinnen van dit gegeven kan tot 20 min van de eerste interactie van de bezoeker met Adobe Target vergen. |
| **(Alleen Adobe Target)** Kan ik een superpubliek maken door klantkenmerkgegevens te combineren met gedeelde publieksgegevens? | Nee. Gegevens voor een gedeeld publiek zijn voltooid. |
| **(Alleen Adobe Target)** Hoe verhoudt de [!DNL customer attributes] -functionaliteit zich tot de Adobe Target-API voor bulkprofielen? | Met de API voor bulkprofielen kunnen Adobe Target-profielen rechtstreeks via de API worden bijgewerkt, voor een afzonderlijk profiel of in bulk. De mogelijkheid is vergelijkbaar met [!DNL customer attributes] , met de volgende belangrijke verschillen:<ul><li>De profiel-API is een REST API-aanroep en [!DNL customer attributes] gebruikt FTP.</li><li>Adobe Target-profiel-API verzendt alleen gegevens naar Adobe Target in plaats van naar de hele Experience Cloud.</li><li>[!DNL customer attributes] biedt een eenvoudige interface voor het maken en beheren van deze externe gegevens.</li></ul> |
| **(Alleen Adobe Target)** Leidt het uploaden van gegevens van [!DNL customer attributes] naar Adobe Target ertoe dat de levensduur van het profiel van de Adobe Target-bezoeker wordt verlengd? | Ja. Zie [ Levensduur van het Profiel van de Bezoeker ](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=nl-NL) in de Hulp van Adobe Target. |
| **(Alleen Adobe Target)** Kan ik me richten op de gegevens die in [!DNL customer attributes] zijn geüpload direct nadat de bezoeker door de klant-id is geïdentificeerd? | Ja. Op de servervraag aan Adobe Target, die mbox derdeidentiteitskaart omvat, zijn alle gegevens van het klantenattribuut beschikbaar. |
| **(Alleen Adobe Target)** Wat vertegenwoordigt de kolom **[!UICONTROL Sync Status]** voor bestanden die zijn geüpload in de kenmerkbron van de klant? | Het aantal records dat door Adobe Target is gepubliceerd en gesynchroniseerd, kan worden weergegeven door het pictogram Synchronisatiestatus te selecteren op basis van een specifiek kenmerkbestand. `Sync %` is een real-time metrisch die het percentage van profielen specificeert die in Adobe Target zijn gesynchroniseerd.<br> **Nota:** het kan tot 24 uren voor attributen aan synchronisatie met Adobe Target vergen. |
| Wat vertegenwoordigen de meetgegevens voor het uploaden van bestanden in [!DNL customer attributes] Source? | U kunt de status controleren van kenmerken die naar [!DNL customer attributes] zijn geüpload met behulp van de volgende meetgegevens: <ul><li>Records: Aantal records in het kenmerkbestand.</li><li>**Nieuwe Verslagen:** Aantal nieuwe verslagen aanwezig in het attributendossier.</li> <li>**Bijgewerkte Verslagen:** Aantal verslagen in die in [!DNL customer attributes] met bijgewerkte waarden in het dossier bestaan.</li><li>**Alle Gegevens (Verslagen):** Totaal aantal met succes geupload verslagen aan [!DNL customer attributes].</li></ul> |

{style="table-layout:auto"}
