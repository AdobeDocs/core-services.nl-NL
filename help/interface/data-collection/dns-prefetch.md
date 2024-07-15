---
description: Leer hoe te om DNS prefetch uit te voeren helpen de tijden van de paginading met verschillende toepassingen en de diensten in Experience Cloud verminderen.
solution: Experience Cloud
title: DNS-prefetch gebruiken
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
source-git-commit: 9ee4d9b0e670dec35cda530892c49e36bf7cc107
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# DNS-prefetch gebruiken

Voer DNS prefetch uit helpen de tijden van de paginading met verschillende toepassingen en de diensten verminderen.

## DNS-prefetch begrijpen

Browsers gebruiken DNS prefetch om domeinnamen automatisch op te lossen die op een Web-pagina aan hun overeenkomstige IP adressen worden verbonden. Het vooraf ingestelde proces wordt gestart wanneer uw browser een webpagina laadt. Stel bijvoorbeeld dat de pagina een selecteerbare koppeling bevat naar `www.adobe.com` . Wanneer browser deze pagina laadt, gebruikt het het [ DNS systeem ](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) om omhoog de verbonden domeinnaam te kijken en het op te lossen aan een overeenkomstig numeriek IP adres. DNS-prefetch verbetert de paginaprestaties omdat de domeinnaam al is omgezet naar een IP-adres voordat een bezoeker van de site op die koppeling of knop klikt. Het DNS-prefetchproces is transparant voor de gebruikers.

## DNS-prefetch en Adobe Experience Cloud-toepassingen

DNS-prefetch werkt automatisch met statische, ingesloten koppelingen op een pagina. Dit betekent ook dat automatische DNS-prefetch niet werkt met verschillende [!UICONTROL Experience Cloud] -toepassingen en -services omdat:

* Elke toepassing of dienst van het Experience Cloud produceert DNS dynamisch vraag aangezien de pagina laadt.
* Browser kan domeinnamen aan IP adres niet oplossen alvorens deze vraag wordt gemaakt.

Nochtans, kunt u DNS prefetch met uw toepassingen van het Experience Cloud manueel uitvoeren. U doet dit door de tag HTML `<dns-prefetch>` toe te voegen aan de sectie `<head>` van de paginacode, zoals hieronder wordt weergegeven. Als de DNS-prefetch correct is geïmplementeerd, kan deze een paar milliseconden lang de laadtijd van de pagina besparen.

## Voorbeelden van DNS-prefetcode

In het volgende voorbeeld ziet u hoe u DNS-prefetchaanroepen naar verschillende [!DNL Experience Cloud] -toepassingen en -services kunt uitvoeren. Voor sommige prefetch-aanroepen is uw [!DNL Adobe] Organisatie-id of informatie over de trackingserver vereist. In deze voorbeelden, vertegenwoordigt de code in *cursief* veranderlijke placeholder. U kunt die code vervangen door uw eigen [!DNL Adobe] partner-id, klantcode of informatie over de trackingserver, enzovoort.

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`.

  Voeg een afzonderlijke tag toe voor elke DNS-naam als u niet-beveiligde en veilige trackingservers gebruikt.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Dienst van identiteitskaart van het Experience Cloud:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">`

* **Advertising Cloud:**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttech.net">`

* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [ DNS Prefetching ](https://www.chromium.org/developers/design-documents/dns-prefetching) op Chromium
