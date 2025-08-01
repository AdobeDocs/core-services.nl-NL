---
title: IP Adressen die door Experience Cloud worden gebruikt
description: Als de firewall van uw organisatie IP-adressen blokkeert die afkomstig zijn van Adobe, gebruikt u deze lijst om uw firewallinstellingen bij te werken.
exl-id: 1fca8d3b-ae8b-4095-96ef-d165f912b4c6
source-git-commit: a18b61cb32286680cb1ab2a296df33509fd95a00
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# IP adressen die door Experience Cloud worden gebruikt

Sommige firewallconfiguraties blokkeren IP-adressen die afkomstig zijn van Adobe-servers voor gegevensverzameling of servers die verantwoordelijk zijn voor de toegang tot gegevens. U kunt deze lijst met bereiken gebruiken om de firewallinstellingen van uw organisatie te wijzigen, zodat u toegang hebt en gegevens kunt verzenden vanuit uw organisatie. Deze pagina omvat zowel binnenkomende systemen (zoals gegevensinzameling) als uitgaande systemen (zoals gegevensvoer in Adobe Analytics) die Adobe gebruikt.

>[!IMPORTANT]
>
>Hoewel Adobe zijn best doet om dit document huidig te houden, kan het niet garanderen dat de lijst van IP waaiers het zelfde blijft. Mogelijke veranderingen omvatten groei en uitbreiding van de zaken, vereist een register van Internet veranderingen in Adobe IP adresruimte, of een dienstverlener van Internet houdt werkend op.

Naast de IP hieronder vermelde adresblokken, hebben de individuele producten van Adobe Experience Cloud hun eigen IP adressen die zij gebruiken:

* [ Adobe Analytics ](https://experienceleague.adobe.com/nl/docs/analytics/technotes/ip-addresses)
* [Customer Journey Analytics](https://experienceleague.adobe.com/nl/docs/analytics-platform/using/technotes/ip-addresses)
* [ Marketo Engage ](https://experienceleague.adobe.com/nl/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo#step-allowlist-marketo-ips)
* [ Adobe Workfront ](https://experienceleague.adobe.com/nl/docs/workfront/using/administration-and-setup/get-started-administration/configure-your-firewall)

## Alle Adobe IP-adresblokken

De volgende lijst behandelt alle IP van Adobe-Bezit adressen. Deze tabel bevat alle Adobe-werknemerskantoren en datacenters die wereldwijd door Adobe worden uitgevoerd. Hieronder vallen geen diensten die op openbare wolken worden gehost.

| IP-blok (CIDR-notatie) |
| --- |
| `63.140.32.0/19` |
| `66.117.16.0/20` |
| `66.235.128.0/19` |
| `130.248.0.0/16` |
| `172.82.192.0/18` |
| `185.34.188.0/22` |
| `192.243.240.0/22` |

{style="table-layout:auto"}

## Adobe Experience Cloud-gegevensverzameling en FTP IP-adresblokken

Als uw organisatie verkiest om specifieke IP adreswaaiers toe te staan, kunt u de volgende lijst van verwijzingen voorzien. Het omvat:

* Servers voor gegevensverzameling voor alle Experience Cloud-producten
* FTP-servers voor alle Experience Cloud-producten

Alle IP waaiers in deze sectie zijn inbegrepen in de bovengenoemde lijst.

| Locatie | IP-bereik (CIDR-notatie) |
| --- | --- |
| Australië | `63.140.55.0/24` |
| Australië | `63.140.56.0/23` |
| California | `63.140.32.0/23` |
| California | `63.140.34.0/24` |
| Frankrijk | `63.140.62.0/23` |
| India | `66.117.22.0/23` |
| Japan | `130.248.169.0/23` |
| Japan | `63.140.50.0/23` |
| Japan | `66.117.31.0/24` |
| Londen | `66.235.156.0/24` |
| Londen | `185.34.188.0/22` |
| Londen | `130.248.152.0/22` |
| Londen | `130.248.244.0/23` |
| Ohio | `66.117.20.0/24` |
| Oregon | `66.235.132.0/22` |
| Oregon | `130.248.130.0/23` |
| Oregon | `130.248.150.0/24` |
| Oregon | `130.248.160.0/21` |
| Oregon | `192.243.242.0/24` |
| Singapore | `130.248.170.0/23` |
| Singapore | `130.248.240.0/24` |
| Singapore | `63.140.44.0/22` |
| Singapore | `63.140.48.0/23` |
| Singapore | `66.117.30.0/24` |
| Singapore | `172.82.240.8/29` |
| Singapore | `172.82.240.88/29` |
| Virginia | `63.140.38.0/23` |
| Virginia | `63.140.54.0/24` |
| Virginia | `67.202.5.244` |

{style="table-layout:auto"}

De Adobe Experience Cloud biedt ook beperkte ondersteuning voor IPv6. Deze IP blokken dienen gelijkaardige doeleinden van de gegevensinzameling als hun IPv4 hierboven tegenhangers, maar omvatten geen FTP.

| Locatie | Host |
| --- | --- |
| Australië | `2406:da1c:406:1a00::/56` |
| Australië | `2406:da1c:ce5:b400::/56` |
| California | `2600:1f1c:366:d900::/56` |
| Frankrijk | `2a05:d012:706:d000::/56` |
| India | `2406:da1a:f34:6a00::/56` |
| Ierland | `2a05:d018:309:600::/56` |
| Japan | `2406:da14:b07:ab00::/56` |
| Ohio | `2600:1f16:130f:7d00::/56` |
| Oregon | `2600:1f14:1eb:7d00::/56` |
| Oregon | `2600:1f14:9d3:2b00::/56` |
| Singapore | `2406:da18:6e8:1e00::/56` |
| Virginia | `2600:1f18:1a20:e800::/56` |
| Virginia | `2600:1f18:4fd:6000::/56` |
| Virginia | `2600:1f18:b00:e100::/56` |
| Virginia | `2600:1f18:d1f:bd00::/56` |

>[!TIP]
>
>FTP-verbindingen voor Adobe Analytics-exportfuncties (waaronder Data Warehouse en gegevensfeeds) zijn alleen afkomstig van IPv4-adressen in de locaties Londen, Oregon en Singapore.
