---
description: Adobe Analytics gebruikt cookies om aanvragen van verschillende browsers te onderscheiden en om nuttige informatie op te slaan die een toepassing later kan gebruiken. Zij kunnen ook worden gebruikt om het doorbladeren informatie aan klantenverslagen te associëren.
keywords: cookies;privacy
seo-description: Adobe Analytics gebruikt cookies om aanvragen van verschillende browsers te onderscheiden en om nuttige informatie op te slaan die een toepassing later kan gebruiken. Zij kunnen ook worden gebruikt om het doorbladeren informatie aan klantenverslagen te associëren.
seo-title: Analysecookies
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Analysecookies
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Analysecookies{#analytics-cookies}

Adobe Analytics gebruikt cookies om aanvragen van verschillende browsers te onderscheiden en om nuttige informatie op te slaan die een toepassing later kan gebruiken. Zij kunnen ook worden gebruikt om het doorbladeren informatie aan klantenverslagen te associëren.

Met name gebruikt Analytics cookies om anoniem nieuwe bezoekers te definiëren, hulp bij het analyseren van gegevens over klikstreams en het bijhouden van historische activiteiten op de website, zoals reactie op bepaalde campagnes of de duur van de verkoopcyclus.

* [Naam cookie: s_ecid](../cookies/cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Naam cookie: AMCV_##@AdobeOrg](../cookies/cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Naam cookie: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Naam cookie: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Naam cookie: s_sq](../cookies/cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Naam cookie: s_vi](../cookies/cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Naam cookie: s_fid](../cookies/cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Cookies ingesteld op plug-ins](../cookies/cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Meer informatie is beschikbaar in de Help bij Analytics over [First Party Cookies](/help/interface/cookies/cookies-first-party.md).

## Naam cookie: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| Kenmerk | Beschrijving |
|--- |--- |
| Opgeslagen informatie | Bevat een kopie van de Experience Cloud ID (ECID) of MID. MID wordt opgeslagen in een sleutelwaardepaar dat deze syntaxis volgt, s_ecid=MCMID | `<ECID>` |
| Verlopen | 2 jaar |
| Gebruik | Dit cookie wordt ingesteld door het domein van de klant nadat het AMCV-cookie door de client is ingesteld. Het doel van dit cookie is het permanent bijhouden van id&#39;s toe te staan in de status van de 1^st^-partij en wordt als referentie-id gebruikt als het AMCV-cookie is verlopen. Kijk hier naar het AMCV-cookie voor meer informatie. |
| Locatie | Alleen CNAME-klanten. Niet van toepassing op scenario&#39;s van derden. Cookie wordt opgeslagen op uw domein, het zelfde domein dat door CNAME en uw het beeldverzoek van Analytics wordt gebruikt. |
| Grootte | 45 bytes |

## Naam cookie: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Kenmerk | Beschrijving |
|--- |--- |
| Opgeslagen informatie | Deze cookie wordt ingesteld en gelezen door de JavaScript-code om te bepalen of cookies zijn ingeschakeld (eenvoudig ingesteld op &quot;Waar&quot;) |
| Verlopen | Dit cookie is een sessiecookie en verloopt wanneer de browser wordt gesloten |
| Gebruik | Slechts één cookie voor alle accounts |
| Locatie | Dit cookie wordt opgeslagen op het domein van de pagina |
| Grootte | 4 bytes |

## Naam cookie: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Kenmerk | Beschrijving |
|--- |--- |
| Opgeslagen informatie | Dit cookie wordt ingesteld en gelezen door de JavaScript-code wanneer de functionaliteit ClickMap of de functionaliteit Activiteitenkaart is ingeschakeld. het bevat informatie over de vorige koppeling waarop de gebruiker heeft geklikt |
| Verlopen | Dit cookie is een sessiecookie en verloopt wanneer de browser wordt gesloten |
| Gebruik | Slechts één cookie voor alle accounts |
| Locatie | Dit cookie wordt opgeslagen op het domein van de pagina |
| Grootte | Varieert afhankelijk van de grootte van pagina URL, maar typisch 100-200 bytes |

## Naam cookie: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Kenmerk | Beschrijving |
|--- |--- |
| Opgeslagen informatie | Unieke tijd-/datumstempel van bezoekersidentiteitskaart |
| Verlopen | 2 jaar |
| Gebruik | Dit cookie wordt gebruikt om een unieke bezoeker te identificeren |
| Locatie | Dit koekje wordt opgeslagen op het domein van het beeldverzoek - typisch een klant-specifiek subdomain onder 2o7.net of omtr dc.net als u derdekoekjes gebruikt, of als uw domein eerderangs koekjes gebruikt. |
| Grootte | 44 bytes |

>[!NOTE]
>
>Elke Analytics-bezoeker-id is gekoppeld aan een bezoekersprofiel op Adobe-servers. Bezoekersprofielen worden na 1 jaar inactiviteit verwijderd, ongeacht de vervaldatum van de cookie van de bezoeker.

## Naam cookie: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Kenmerk | Beschrijving |
|--- |--- |
| Opgeslagen informatie | Unieke tijd-/datumstempel van bezoekersidentiteitskaart voor alternatieven |
| Verlopen | 2 jaar |
| Gebruik | Dit cookie wordt gebruikt om een unieke bezoeker te identificeren als de standaardcookie niet beschikbaar is vanwege cookie-beperkingen van derden. `s_vi` Niet gebruikt voor implementaties die cookies van de eerste fabrikant gebruiken. |
| Locatie | Dit cookie wordt op uw domein opgeslagen als een cookie van de eerste fabrikant. |
| Grootte | 33 bytes |

## Cookie-markeringen

In de volgende tabel worden de vlaggen voor Analytics-cookies beschreven:

| Koekje (ingesteld door) | httpOnly | Beveiligen | SameSite |
|--- |--- |--- |--- |
| s_vi (http Response) | Nee | Ja wanneer SameSite &quot;None&quot; is en verbinding HTTPS gebruikt | Standaard &#39;Lax&#39; wanneer CNAME wordt gebruikt. &quot;Geen&quot; bij gebruik van 2o7.net of omtr dc.net. |
| s_ecid (http Response) | Nee | Nee | &quot;Lax&quot; |
| s_fid (JavaScript) | Nee | Nee | Ongedaan maken |
| s_cc (JavaScript) | Nee | Nee | Ongedaan maken |
| s_sq (JavaScript) | Nee | Nee | Ongedaan maken |

>[!NOTE] Als het gebruiken van één enkele CNAME aan spoor over veelvoudige domeinen of eigenschappen, zou SameSite aan &quot;niets&quot;voor moeten worden geplaatst `s_vi`. Neem contact op met de klantenservice voor hulp bij het wijzigen van de cookie-instellingen van Analytics.

## Cookies ingesteld op plug-ins {#section-a6b1cae8454945fab9eea5c7884c40fc}

Afhankelijk van het gebruik van plug-ins voor Analytics kunnen extra cookies worden ingesteld. Deze cookies zijn codefragmenten die beschikbaar zijn voor de client en die onder verschillende omstandigheden kunnen worden gebruikt. Deze omstandigheden omvatten: waarden ophalen van de URL; samenvoegen van waarden die aan Analytics moeten worden doorgegeven; vastleggen van het verlaten van formulieren enzovoort. Neem contact op met ClientCare voor specifieke informatie over cookies die door elke insteekmodule worden ingesteld. Een voorbeeld hiervan is het [!DNL s_vh] cookie dat wordt gebruikt met de insteekmodules *Eenmaal instellen per* en Laatste waarde ** instellen en ophalen.

Conversievariabelen (eVarX) die zonder JavaScript in een afbeeldingsaanvraag zijn ingevoerd, zoals code die in een e-mailbericht is geplaatst, worden alleen correct toegewezen als de e-mailclient en webbrowser dezelfde cookieruimte delen.