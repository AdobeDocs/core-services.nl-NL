---
description: Beheerders kunnen meer weten over de vereisten en wat ze moeten verwachten als ze een upgrade uitvoeren naar Analytics Premium en waar ze hulp kunnen vinden als beheerder van de Experience Cloud.
keywords: upgrading
seo-description: Beheerders kunnen meer weten over de vereisten en wat ze moeten verwachten als ze een upgrade uitvoeren naar Analytics Premium en waar ze hulp kunnen vinden als beheerder van de Experience Cloud.
seo-title: Upgrade uitvoeren naar Analytics Premium en Experience Cloud
solution: Experience Cloud
title: Upgrade uitvoeren naar Analytics Premium en Experience Cloud
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Upgrade uitvoeren naar Analytics Premium en Experience Cloud

Beheerders kunnen meer weten over de vereisten en wat ze moeten verwachten als ze een upgrade uitvoeren naar Analytics Premium en waar ze hulp kunnen vinden als beheerder van de Experience Cloud.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Als u een upgrade uitvoert naar Adobe Analytics Premium, beschikt u over alle mogelijkheden of producten die beschikbaar zijn op het gebied van Analytics Standard, zoals Data Warehouse, Ad hoc Analyse, Report Builder en Data Connectors. (Deze producten zijn afzonderlijk verkocht aan klanten die de puntoplossing, SiteCatalyst, gebruiken.)

De Analytics Premium biedt u:

* Toegang tot 250 conversievariabelen (eVars)
* [Mobiele App Analytics](https://docs.adobe.com/content/help/en/mobile-services/using/home.html)
* Data Workbench (Visual data query; op regels gebaseerde toerekening; kanaalanalyse)

>[!NOTE]
>
>Geen migratie is nodig bij upgrades, maar u dient rekening te houden met een aantal aspecten:
>
>* De eVars 76-250 (SiteCatalyst) en 100-250 (Standaard) zijn zichtbaar in de beheerprogramma&#39;s, maar worden nog niet ingeschakeld.>
>* Adobe schakelt bijdrageanalyse in. De locatie verandert niet (deze is nog steeds beschikbaar op de pagina Anomaly Detection), maar nu wordt automatisch begonnen met het analyseren van alle gegevenspunten.>


## Analyse Premium voltooid {#section_BFAD815EDF364845A52B340B2FD5B64C}

In de Premium Analytics-versie is de volledige functionaliteit van [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)beschikbaar, plus de volgende upgrades:

| Product | Upgrades |
|--- |--- |
| Rapporten en analyses | <ul><li>[Bijdrage-analyse](https://docs.adobe.com/content/help/en/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html)</li><li>[Klantkenmerken](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (maximaal 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmic Attribution</li><li>Vooraf gebouwde werkruimten</li></ul> |
| Analyseplatform | [Live stream](https://helpx.adobe.com/analytics/kb/getting-started-with-livestream-api.html) (onbewerkte gegevens, dashboards, triggers) |

## Voorspelende inlichtingen {#section_B407932C07A7476F83FB0275C3FB63DC}

Door de upgrade naar Predictive Intelligence wordt [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus ingeschakeld:

| Product | Upgrades |
|---|---|
| Rapporten en analyses | [Bijdrage-analyse](https://docs.adobe.com/content/help/en/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html) |
| Data Workbench | Vooraf gebouwde werkruimten voor publiekskwalificaties en voorspellende marketing. |
| Analyseplatform | Live stream (dashboards en triggers) |

## Klant 360 {#section_3B2AC245388248688067DC9A48957AFB}

Upgrade naar Customer 360 biedt [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Product | Upgrades |
|--- |--- |
| [Klantkenmerken](../attributes/attributes.md) | Kenmerken van de klant (analyse en segmentdeling) |
| Data Workbench | <ul><li>Afgeleide klantkenmerken</li><li>Vooraf gebouwde werkruimten voor publieksdetectie</li></ul> |
| Analyseplatform | [Klantkenmerken](../attributes/attributes.md) |

## Geavanceerde kenmerken {#section_9E4986A8389946CCAA7D003268343296}

Geavanceerde Attributie biedt toegang tot [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus Algorithmic Attribution in Data Workbench (25% server call volume).

## Vereisten voor Data Workbench {#section_D959CA68D6DB42C38707F8E0CA3654CC}

De ondersteunde gebruikers kunnen via e-mail verzoeken dat alle clientlicenties worden bijgewerkt om de Premium weer te geven `dwb@adobe.com`. Dit laat eigenschappen zoals Algorithmic Attribution toe.

TechOps zal uw contractverplichting herzien en de juiste beheerde infrastructuur bepalen, die capaciteit verhoogt of vermindert, en dan zullen zij met u, door de Manager van de Rekening of het raadplegen, coördineren om het even welke veranderingen op te stellen.

Alle software die op locatie wordt uitgevoerd, moet worden gedeactiveerd. Dit geldt ook voor sensoren. Dit betekent dat u ervoor moet zorgen dat de gegevens op de juiste wijze worden bijgehouden via de analysetags.

## Ervaar cloud - Gebruikers en producten beheren {#section_6471C54454024301B2E0B687F79F6738}

De de Cloud en kerndiensten van de ervaring zijn beschikbaar aan gebruikers van de Norm van de Analyse en van de Premie, op voorwaarde dat u de implementatie die in [Aan de slag wordt beschreven hebt gevolgd - laat uw oplossingen voor de kerndiensten](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)toe. (Dat proces helpt u uw implementatie te moderniseren, en laat u toe om en beheerder in de Wolk van de Ervaring te worden.)

Nadat u zich hebt aangemeld bij de Experience Cloud, kunt u zich aanmelden via de Experience Cloud op [!DNL experiencecloud.adobe.com] en beginnen met het gebruik van de basisservices (inclusief klantkenmerken, publiek en analytische gegevens voor de mobiele app).

### Gebruikers en groepen beheren

Gebruikersbeheer wordt uitgevoerd in de [Adobe Admin Console](https://helpx.adobe.com/enterprise/help/aedash.html) (productkoppeling).

U kunt een 1:1-kaart instellen tussen een groep die is gemaakt in de Adobe Admin Console en een oplossingsgroep (zoals Adobe Analytics). Hierna wordt voor een nieuwe gebruiker die aan de toegewezen beheerconsole-groep is toegevoegd, automatisch een account voor de analyseoplossing gemaakt en gekoppeld aan de Adobe-id van de gebruiker. (Bestaande gebruikers moeten hun gegevens van de oplossingsaccount handmatig koppelen aan toegangsoplossingen via de aanmeldingsgegevens voor de Experience Cloud.)

>[!NOTE]
>
>U kunt meerdere oplossingsgroepen toewijzen aan één beheerconsole-groep. Adobe raadt echter een-op-een-toewijzing aan. Wanneer u de groepen van tevoren toewijst, kunt u meerdere gebruikers uitnodigen, maken, machtigingen en toevoegen door een CSV te uploaden.
