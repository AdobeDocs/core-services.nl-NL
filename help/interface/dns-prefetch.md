---
description: Leer hoe te om DNS prefetch uit te voeren helpen de tijden van de paginading met verschillende oplossingen en de diensten in Experience Cloud verminderen.
solution: Experience Cloud
title: 'DNS-prefetch gebruiken met verschillende oplossingen en services '
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
feature: '"Klantkenmerken, Audience Library, Admin Console"'
topic: Beheer
role: Beheerder
level: Ervaren
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 1%

---


# DNS-prefetch gebruiken met verschillende oplossingen en services

Voer DNS prefetch uit helpen de tijden van de paginading met verschillende oplossingen en de diensten verminderen.

## DNS-prefetch {#section_772BF9CB7C4141DE9B0355146E2CD962}

Browsers gebruiken DNS prefetch om domeinnamen automatisch op te lossen die op een Web-pagina aan hun overeenkomstige IP adressen worden verbonden. Het vooraf ingestelde proces wordt gestart wanneer uw browser een webpagina laadt. Als voorbeeld, zeg uw pagina een klikbare verbinding aan `www.adobe.com` bevat. Wanneer browser deze pagina laadt, gebruikt het [DNS systeem](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) om omhoog de verbonden domeinnaam te kijken en het op te lossen aan een overeenkomstig numeriek IP adres. DNS-prefetch verbetert de paginaprestaties omdat de domeinnaam al is omgezet naar een IP-adres voordat een bezoeker van de site op die koppeling of knop klikt. Het DNS-prefetchproces is transparant voor de gebruikers.

## DNS-prefetch- en Adobe Experience Cloud-oplossingen {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

DNS-prefetch werkt automatisch met statische, ingesloten koppelingen op een pagina. Dit betekent ook dat automatische DNS-prefetch niet werkt met verschillende [!UICONTROL Experience Cloud] oplossingen en services omdat:

* Elke oplossing of de dienst van Experience Cloud produceert dynamisch DNS vraag aangezien de pagina laadt.
* Browser kan domeinnamen aan IP adres niet oplossen alvorens deze vraag wordt gemaakt.

Nochtans, kunt u DNS prefetch met uw oplossingen van Experience Cloud manueel uitvoeren. U doet dit door de HTML `<dns-prefetch>` markering aan de `<head>` sectie van uw paginacode zoals hieronder getoond toe te voegen. Als de DNS-prefetch correct is geïmplementeerd, kan deze een paar milliseconden lang de laadtijd van de pagina besparen.

## DNS-voorbeeldcode {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

De volgende voorbeelden tonen u hoe te om DNS prefetch vraag aan verschillende [!DNL Experience Cloud] oplossingen en de diensten te maken. Voor sommige prefetch-aanroepen is uw [!DNL Adobe] Organisatie-id of informatie over de trackingserver vereist. In deze voorbeelden vertegenwoordigt de code in *italics* een variabele placeholder. U vervangt die code door uw eigen [!DNL Adobe] partner-id, klantcode of serverinformatie, enz.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   Voeg een afzonderlijke tag toe voor elke DNS-naam als u niet-beveiligde en veilige trackingservers gebruikt.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID-service:partner-id hier** `<link rel="dns-prefetch" href="//fast. *`invoegen`*.demdex.net">`

* **Dynamisch tagbeheer**  (DTM): Niet vereist. DTM-koppelingen zijn beschikbaar zodra de pagina wordt geladen.

* **Media optimaliseren (Ad Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **[!DNL Target]:** `<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [DNS-prefettering](https://www.chromium.org/developers/design-documents/dns-prefetching)

