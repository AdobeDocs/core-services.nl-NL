---
description: Leer meer over de vereisten en wat u kunt verwachten als u een upgrade uitvoert naar de Analytics Premium.
keywords: Adobe Analytics Premium-upgrade
solution: Experience Cloud
title: 'Upgrade naar Analytics Premium en de Experience Cloud '
topic: Beheer
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
feature: Admin Console
role: Administrator
level: Experienced
exl-id: 746d396d-9629-42db-8c55-07d2d24e4611
source-git-commit: ebefd433e96da422674e7ee71c8988d4011fed11
workflow-type: tm+mt
source-wordcount: '616'
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

In de Premie van Analytics voltooit, krijgt u alle mogelijkheden van [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus de volgende verbeteringen:

| Product | Upgrades |
|--- |--- |
| Rapporten en analyses | <ul><li>[Contributieanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en)</li><li>[Klantkenmerken](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)  (maximaal 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmic Attribution</li><li>Vooraf gebouwde werkruimten</li></ul> |
| Platform Analytics | [Live stream](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/live-stream-api/index.md)  (onbewerkte gegevens, dashboards, triggers) |

## Voorspelende inlichtingen {#section_B407932C07A7476F83FB0275C3FB63DC}

Door de upgrade naar Predictive Intelligence wordt [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Product | Upgrades |
|---|---|
| Rapporten en analyses | [Contributieanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en) |
| Data Workbench | Vooraf gebouwde werkruimten voor publiekskwalificaties en voorspellende marketing. |
| Platform Analytics | Live stream (dashboards en triggers) |

## Klant 360 {#section_3B2AC245388248688067DC9A48957AFB}

Upgraden naar Klant 360 biedt [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Product | Upgrades |
|--- |--- |
| [Klantkenmerken](attributes.md) | Kenmerken van de klant (analyse en segmentdeling) |
| Data Workbench | <ul><li>Afgeleide klantkenmerken</li><li>Vooraf gebouwde werkruimten voor publieksdetectie</li></ul> |
| Platform Analytics | [Klantkenmerken](attributes.md) |

## Geavanceerde kenmerken {#section_9E4986A8389946CCAA7D003268343296}

Geavanceerde Attributie biedt toegang tot [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus Algorithmic Attribution in Data Workbench (25% server call volume).

## Data Workbench-eisen {#section_D959CA68D6DB42C38707F8E0CA3654CC}

De ondersteunde gebruiker(s) kunnen via een e-mail `dwb@adobe.com` verzoeken dat alle clientlicenties worden bijgewerkt om de Premium te weerspiegelen. Deze update schakelt functies zoals Algorithmic Attribution in.

TechOps herziet uw contractverplichting en bepaalt de juiste beheerde infrastructuur, die capaciteit verhoogt of vermindert, en dan coördineren zij met u, door de Manager van de Rekening of het raadplegen, om het even welke veranderingen op te stellen.

Alle software die op locatie wordt uitgevoerd, moet worden gedeactiveerd. Deze software bevat sensoren. Dit betekent dat u ervoor moet zorgen dat de [!DNL Analytics]-tags correct worden bijgehouden.

## Experience Cloud - Gebruikers en producten beheren {#section_6471C54454024301B2E0B687F79F6738}

Experience Cloud- en kernservices zijn beschikbaar voor gebruikers van Analytics Standard en Premium als u de modernisering van de implementatie hebt gevolgd die wordt beschreven in [Aan de slag - uw oplossingen inschakelen voor kernservices](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (Dat proces helpt u uw implementatie moderniseren, en laat u toe om en beheerder in Experience Cloud te worden.)

Nadat u zich bij de Experience Cloud hebt aangemeld, kunt u zich aanmelden via de Experience Cloud op [!DNL experience.adobe.com] en beginnen met het gebruik van de kernservices (inclusief klantkenmerken, soorten publiek en analytische toepassingen voor mobiele apparaten).

### Gebruikers en groepen beheren

Gebruikersbeheer wordt uitgevoerd in [Adobe Admin Console](https://helpx.adobe.com/nl/enterprise/using/admin-console.html) (productkoppeling).

U kunt een 1:1-kaart instellen tussen een groep die in de Adobe Admin Console is gemaakt en een oplossingsgroep (zoals Adobe Analytics). Hierna heeft een nieuwe gebruiker die aan de toegewezen groep Admin Consoles is toegevoegd, automatisch een account voor de analytische oplossing die aan de Adobe ID van de gebruiker is gekoppeld. (Bestaande gebruikers moeten hun gegevens van de oplossingsaccount handmatig koppelen aan toegangsoplossingen via de Experience Cloud-aanmelding.)

>[!NOTE]
>
>U kunt verscheidene oplossingsgroepen aan één groep van de Admin Console in kaart brengen. Adobe raadt echter een-op-een-toewijzing aan. Wanneer u de groepen van tevoren toewijst, kunt u meerdere gebruikers uitnodigen, maken, machtigingen en toevoegen door een CSV te uploaden.