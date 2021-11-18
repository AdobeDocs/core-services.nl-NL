---
description: Leer meer over de vereisten en wat u kunt verwachten als u een upgrade uitvoert naar de Analytics Premium.
keywords: Adobe Analytics Premium-upgrade
solution: Experience Cloud
title: 'Upgrade naar Analytics Premium en de Experience Cloud '
topic: Administration
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
feature: Admin Console
role: Admin
level: Experienced
exl-id: 746d396d-9629-42db-8c55-07d2d24e4611
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 3%

---

# Upgrade uitvoeren naar Analytics Premium en de Experience Cloud

Beheerders kunnen meer weten over de vereisten en wat ze moeten verwachten als ze een upgrade uitvoeren naar Analytics Premium en waar ze hulp kunnen zoeken als beheerder van een Experience Cloud.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Als u een upgrade uitvoert naar Adobe Analytics Premium, beschikt u over alle mogelijkheden of producten die beschikbaar zijn op de standaard Analytics, waaronder Data Warehouse, Ad Hoc Analysis, Report Builder en Gegevensconnectors.

De Analytics Premium biedt u:

* Toegang tot 250 conversievariabelen (eVars)
* [Mobiele App Analytics](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=en)
* Data Workbench (vragen van visuele gegevens; op regels gebaseerde toerekening; kanaalanalyse)

>[!NOTE]
>
>Geen migratie is nodig bij upgrades, maar u dient rekening te houden met een aantal aspecten:
>
>* De eVars 76-250 en 100-250 (Standaard) zijn zichtbaar in de Hulpmiddelen Admin, maar zijn niet toegelaten.
>* De analyse van de bijdrage wordt aangezet door Adobe. De locatie verandert niet (deze is nog steeds beschikbaar op de pagina Anomaly Detection), maar het analyseert automatisch alle gegevenspunten.


## Analyse Premium voltooid {#section_BFAD815EDF364845A52B340B2FD5B64C}

In Analytics Premium Complete beschikt u over alle mogelijkheden van [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus de volgende upgrades:

| Product | Upgrades |
|--- |--- |
| Rapporten en analyses | <ul><li>[Contributieanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en)</li><li>[Klantkenmerken](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (Maximaal 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmic Attribution</li><li>Vooraf gebouwde werkruimten</li></ul> |
| Platform Analytics | [Live stream](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/live-stream-api/index.md) (onbewerkte gegevens, dashboards, triggers) |

{style=&quot;table-layout:auto&quot;}

## Voorspelende inlichtingen {#section_B407932C07A7476F83FB0275C3FB63DC}

Door te upgraden naar voorspellende intelligentie [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Product | Upgrades |
|---|---|
| Rapporten en analyses | [Contributieanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en) |
| Data Workbench | Vooraf gebouwde werkruimten voor publiekskwalificaties en voorspellende marketing. |
| Platform Analytics | Live stream (dashboards en triggers) |

{style=&quot;table-layout:auto&quot;}

## Klant 360 {#section_3B2AC245388248688067DC9A48957AFB}

Upgrade naar 360 aanbiedingen van de Klant [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Product | Upgrades |
|--- |--- |
| [Klantkenmerken](attributes.md) | Kenmerken van de klant (analyse en segmentdeling) |
| Data Workbench | <ul><li>Afgeleide klantkenmerken</li><li>Vooraf gebouwde werkruimten voor publieksdetectie</li></ul> |
| Platform Analytics | [Klantkenmerken](attributes.md) |

{style=&quot;table-layout:auto&quot;}

## Geavanceerde kenmerken {#section_9E4986A8389946CCAA7D003268343296}

Geavanceerde kenmerken bieden toegang tot [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus Algorithmic Attribution in Data Workbench (25% server call volume).

## Data Workbench-eisen {#section_D959CA68D6DB42C38707F8E0CA3654CC}

De ondersteunde gebruikers kunnen via e-mail verzoeken dat alle clientlicenties worden bijgewerkt met de Premium `dwb@adobe.com`. Deze update schakelt functies zoals Algorithmic Attribution in.

TechOps herziet uw contractverplichting en bepaalt de juiste beheerde infrastructuur, die capaciteit verhoogt of vermindert, en dan coördineren zij met u, door de Manager van de Rekening of het raadplegen, om het even welke veranderingen op te stellen.

Alle software die op locatie wordt uitgevoerd, moet worden gedeactiveerd. Deze software bevat sensoren, wat betekent dat u voor een juiste tracking moet zorgen via [!DNL Analytics] -tags.

## Experience Cloud - Gebruikers en producten beheren {#section_6471C54454024301B2E0B687F79F6738}

Experience Cloud- en kernservices zijn beschikbaar voor gebruikers van Analytics Standard en Premium als u de in [Aan de slag - uw toepassingen inschakelen voor kernservices](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (Dat proces helpt u uw implementatie moderniseren, en laat u toe om en beheerder in Experience Cloud te worden.)

Nadat u zich bij de Experience Cloud aansluit, kunt u login via de Experience Cloud bij [!DNL experience.adobe.com] en beginnen met het gebruik van kernservices (inclusief klantkenmerken, publiek en mobiele toepassingsanalysemogelijkheden).

### Gebruikers en groepen beheren

Gebruikersbeheer wordt uitgevoerd in het dialoogvenster [Adobe Admin Console](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) (productkoppeling).

U kunt een 1:1-kaart instellen tussen een groep die in de Adobe Admin Console is gemaakt en een oplossingsgroep (zoals Adobe Analytics). Hierna heeft een nieuwe gebruiker die aan de toegewezen groep Admin Consoles is toegevoegd, automatisch een account voor de toepassing Analytics gemaakt en gekoppeld aan de Adobe ID van de gebruiker. (Bestaande gebruikers moeten hun aanmeldingsgegevens van hun toepassingsaccount handmatig koppelen aan toepassingen via de Experience Cloud-aanmelding.)

>[!NOTE]
>
>U kunt meerdere toepassingsgroepen toewijzen aan één groep Admin Consoles. Adobe raadt echter een-op-een-toewijzing aan. Wanneer u de groepen van tevoren toewijst, kunt u meerdere gebruikers uitnodigen, maken, machtigingen en toevoegen door een CSV te uploaden.
