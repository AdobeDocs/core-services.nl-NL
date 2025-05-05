---
description: Leer meer over Adobe Advertising cookies voor het toewijzen en plaatsen van afspraken aan conversiegebeurtenissen en gebruik deze informatie mogelijk om advertenties te optimaliseren.
title: Cookies Adoben Advertising
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# Cookies Adoben Advertising

Adobe Advertising (voorheen Adobe Advertising Cloud) gebruikt cookies om gebeurtenissen voor conversie in kaart te brengen en te koppelen aan conversiegebeurtenissen en deze informatie mogelijk te gebruiken om advertenties te optimaliseren.

>[!NOTE]
>
>De markering van Javascript van de bèta-Adobe Advertising die de [ identiteitskaart van Adobe Experience Cloud (ECID) Dienst ](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=nl-NL) gebruikt leidt tot eerste-partij [ Experience Cloud ](experience-cloud.md) `s_ecid` koekjes, niet de koekjes van de Adobe Advertising.

| Naam cookie | Verlopen | Grootte | Locatie | Beschrijving |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15 minuten | 52 bytes | `everesttech.net` | Hiermee slaat u id&#39;s en tijdstempels van weergaveklikken op. Hiermee wordt bepaald of een klikgebeurtenis op een weergaveadvertentie van toepassing is op een Adobe Analytics-hit. |
| **`_tmae`** | 1 jaar | 1 kB | `everesttech.net` | Hiermee slaat u gecodeerde id&#39;s en tijdstempels voor advertentieopdrachten op met DSP bijhouden. Omvat gebruikersbetrokkenheid bij advertenties, zoals de laatst bekeken advertentie |
| **`_tmid`** | 1 jaar | ~20 bytes | `everesttech.net` | Hiermee wordt de Demand Side Platform-id (DSP) van de Adobe Advertising opgeslagen. Komt overeen met de bezoeker-id in het `everest_g_v2` -cookie. |
| **`adcloud`** | 1 jaar | 50-150 bytes | Eerste partij | De tijdstempels van het laatste bezoek van de bezoeker aan uw website en de laatste zoekklik van de bezoeker. Hiermee slaat u ook de `ef_id` op die is gemaakt toen de bezoeker op een advertentie klikte. Verdeelt de bezoekersidentiteitskaart met relevante publiekssegmenten en omzettingen. Hiermee kunt u de laadtijden van pagina&#39;s optimaliseren door overbodige verzoeken om Adobe te voorkomen. |
| **`ev_sync_*`** |  | 8 bytes | `everesttech.net` | De datum waarop synchronisatie wordt uitgevoerd in `yyymmdd` -indeling. Synchroniseert de bezoeker-id van de Adobe Advertising met de partner en de uitwisseling. Het wordt gecreeerd voor nieuwe bezoekers en verzendt een synchronisatieverzoek wanneer verlopen. Bevat de cookies `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm` en `ev_sync_yh`. |
| **`everest_g_v2`** | 1 jaar | ~27 bytes | `everesttech.net` | Hiermee slaat u de browser en de bezoeker-id op. Gemaakt nadat een gebruiker in eerste instantie op een advertentie klikt. Wordt gebruikt om de huidige en volgende muisklikken toe te wijzen aan andere gebeurtenissen op uw website. |
| **`everest_session_v2`** | Sessie | ~16 bytes | `everesttech.net` | Hiermee slaat u de huidige sessie-id op. |
| **`id_adcloud`** | 91 dagen | 16 bytes | Eerste partij | Hiermee slaat u de bezoeker-id op. |

{style="table-layout:auto"}
