---
description: Meer weten over Adobe Analytics cookies in Adobe Experience Cloud?
solution: Analytics
title: Adobe Analytics Cookies
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: d3a559ca2f7963256d48a25cd51099edb5e3fe76
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Adobe Analytics cookies

Adobe Analytics gebruikt cookies om aanvragen van verschillende browsers te onderscheiden en om nuttige informatie op te slaan die een toepassing later kan gebruiken. Zij kunnen ook worden gebruikt om het doorbladeren informatie met klantenverslagen te associëren.

Analytics gebruikt cookies om nieuwe bezoekers anoniem te definiëren, hulp bij het analyseren van gegevens over klikstreams en het bijhouden van historische activiteiten op de website, zoals het reageren op bepaalde campagnes of de duur van de verkoopcyclus.

| Naam cookie | Verlopen | Grootte | Locatie | Beschrijving |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 13 maanden | 45 bytes | Eerste partij | Hiermee slaat u de Experience Cloud-id (ECID) of MID op. Instellen op HTTP-reactie. De MID wordt opgeslagen in de `s_ecid=MCMID` -indeling. Stel deze waarde in nadat de client het AMCV-cookie heeft ingesteld. Het staat blijvende het volgen van eerste-partijidentiteitskaart toe en als verwijzingsID wordt gebruikt als het koekje AMCV verloopt. `SameSite` is ingesteld op Lax. Als u de SDK van het Web gebruikt om Adobe Analytics uit te voeren, wordt de koekjesvervalsing geplaatst aan 2 jaar; nochtans, korten de meeste moderne browsers de vervaldatum tot 13 maanden af. |
| **`s_cc`** | Sessie | 4 bytes | Eerste partij | Hiermee bepaalt u of cookies zijn ingeschakeld. Ingesteld door JavaScript. |
| **`s_sq`** | Sessie | 100-200 bytes | Eerste partij | Wordt gebruikt door Activity Map. Deze bevat informatie over de vorige koppeling waarop de bezoeker heeft geklikt. Ingesteld door JavaScript. |
| **`s_vi`** | 2 jaar | 44 bytes | First-party of `*.omtrdc.net` (derde) | Hiermee worden een unieke bezoeker-id en een unieke tijdstempel opgeslagen. Instellen op HTTP-reactie. Elke bezoeker-id is gekoppeld aan een bezoekersprofiel op Adobe-servers. Bezoekersprofielen worden na 1 jaar inactiviteit verwijderd, ongeacht de vervaldatum van de cookie van de bezoeker. De markering `Secure` wordt ingesteld wanneer `SameSite` &quot;Geen&quot; is en de verbinding HTTPS is. `SameSite` is standaard &quot;Lax&quot; voor cookies van de eerste partij. `SameSite` is &quot;Geen&quot; bij gebruik van cookies van derden, zoals op `omtrdc.net` of `2o7.net` . Stel `SameSite` in op &quot;Geen&quot; wanneer u één CNAME gebruikt om meerdere domeinen of eigenschappen bij te houden. |
| **`s_fid`** | 2 jaar | 33 bytes | Eerste partij | Hiermee slaat u de fallback-unieke bezoeker-id en het tijdstempel op. Wordt ingesteld door JavaScript als de standaard `s_vi` -cookie niet kan worden ingesteld vanwege cookie-beperkingen van derden. Niet gebruikt voor cookie-implementaties van de eerste fabrikant. |
| **`s_ac`** | Meteen | 1 byte | Eerste partij | Hiermee bepaalt u het juiste domein voor het instellen van AppMeasurement-cookies. Bevat de statische waarde `"1"` . Zodra deze cookie is ingesteld, wordt deze direct verwijderd. |

## Cookies ingesteld op plug-ins

Sommige implementaties maken gebruik van plug-ins. Dit zijn codefragmenten die aanvullende functionaliteit bieden voor Analytics. Deze plug-ins kunnen cookies instellen die hierboven niet worden vermeld. Zie [ het overzicht van stop-ins van Analytics ](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) voor een lijst van beschikbare stop-ins en welke koekjes die zij plaatsen.

## Gevolgen van het verwijderen van Analytics-cookies

Als een bezoeker zijn of haar Analytics-cookies verwijdert, kunt u het volgende overwegen:

* **de identificatie van de Bezoeker wordt verloren:** wanneer de koekjes worden geschrapt, kan Adobe Analytics terugkerende bezoekers niet erkennen. De volgende keer dat de gebruiker uw site bezoekt, wordt deze geteld als een nieuwe bezoeker. [ dwars-apparaat Analytics ](https://experienceleague.adobe.com/en/docs/analytics/components/cda/overview) kan helpen dit effect verlichten.
* **de continuïteit van de Zitting is gebroken:** om het even welke op zitting-gebaseerde of multi-bezoek analyse (zoals attributie of omzetting het volgen) wordt onderbroken. Gebeurtenissen en conversies die na het verwijderen van cookies plaatsvinden, kunnen door dezelfde gebruiker niet aan eerdere activiteiten worden gekoppeld.
* **Personalization en de segmentatie worden beïnvloed:** Segmenten of gepersonaliseerde ervaringen die op de geschiedenis of het gedrag van de bezoeker worden gebaseerd worden teruggesteld, aangezien het vorige gegeven niet meer met hun huidige bezoek wordt geassocieerd.
* **het dwars-domein volgen wordt onderbroken:** voor derdekoekjes, die hen schrappen verhindert Adobe Analytics gebruikersactiviteit over veelvoudige domeinen te verbinden die u bezit.
