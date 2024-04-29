---
description: Leer hoe u beveiligde certificaten instelt voor gebruik met Adobe Experience Cloud-cookies van de eerste fabrikant.
solution: Experience Cloud,Analytics
title: Certificaatprogramma met beheerde Adobe
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 2691f0dc91e48a8f817467e334d9028f2e506e70
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Certificaatprogramma met beheerde Adobe

Het Adobe-beheerde certificaatprogramma is het geadviseerde proces voor vestiging eerste-partijcertificaten nodig voor een implementatie CNAME. Het programma wordt volledig geautomatiseerd zodra dit is geconfigureerd. De certificaten worden tijdig vernieuwd, zodat gegevensverzameling niet wordt beïnvloed door verlopen certificaten. Het programma is gratis voor de eerste 100 CNAME&#39;s.

Als u momenteel uw eigen certificaten beheert, bent u verantwoordelijk voor het aanschaffen, onderhouden en opgeven van een certificaat voor Adobe voor cookie van andere bedrijven. U kunt contact opnemen met de klantenservice van de Adobe om de migratie naar het door Adobe beheerde certificaatprogramma te bespreken.

## Implementatie

Ga als volgt te werk om een nieuw certificaat voor gegevensverzameling van de eerste partij te implementeren:

1. Download en vul de [Formulier voor eerste domeinaanvraag](cookies/assets/First_Party_Domain_Request_Form.xlsx)

1. Open een kaartje met de Zorg van de Klant van de Adobe die om de inzameling van de eerste-partijgegevens over het Adobe-beheerde certificaatprogramma verzoekt te plaatsen.

1. Op het ontvangen van het kaartje, voorziet de vertegenwoordiger van de Adobe u van een verslag CNAME. Deze verslagen moeten op DNS server van uw bedrijf worden gevormd alvorens de Adobe het certificaat namens u kan kopen. De hostnaam `data.example.com` punten naar `hiodsibxvip01.data.adobedc.net`.

1. Wanneer de CNAME-record op de servers van uw organisatie is geïnstalleerd, werkt de Adobe samen met DigiCert om een certificaat aan te schaffen en te installeren op servers voor gegevensverzameling van Adoben.

## Hostnaam valideren door:sturen {#validate}

Nadat Adobe het certificaat heeft geïnstalleerd, kunt u een van de volgende methoden gebruiken om te controleren of het werkt.

+++**Browservalidatie**

Met elke browser kunt u controleren of een certificaat correct is geïnstalleerd. Typ uw NAAM met `_check` als het pad naar de adresbalk. Bijvoorbeeld:

`data.example.com/_check`

Als alles werkt, wordt in de browser `SUCCESS`. Als het certificaat niet correct is geïnstalleerd, krijgt u een beveiligingswaarschuwing.

+++

+++**Opdrachtregel (`curl`)**

De meeste moderne besturingssystemen hebben al [`curl`](https://curl.se) geïnstalleerd.

Typ het volgende op de opdrachtregel:

```sh
curl data.example.com/_check
```

Als alles correct werkt, keert de console terug `SUCCESS`.

>[!TIP]
>
>U kunt de `-k` markering om de veiligheidswaarschuwing onbruikbaar te maken om met het oplossen van problemen te helpen.

+++

+++**Opdrachtregel (`nslookup`)**

Typ het volgende op de opdrachtregel:

```sh
nslookup data.example.com
```

Als alles correct werkt, zijn de servers van de gegevensinzameling van de Adobe teruggekeerd:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: smetrics.example.com
```

+++

## Implementatiecode bijwerken {#update}

Nadat u hebt bevestigd dat het certificaat correct werkt, kunt u de Adobe-implementatie bijwerken en deze waarden gebruiken.

* Voor Adobe Analytics AppMeasurement-implementaties werkt u de [`trackingServer`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserver) configuratievariabele. Als u een bestaande implementatie hebt, raadpleegt u [Bezoekersmigratie](https://experienceleague.adobe.com/en/docs/analytics/technotes/visitor-migration) voor aanvullende stappen om te voorkomen dat bestaande bezoekers worden geteld als nieuwe bezoekers.
* Voor Web SDK-implementaties werkt u de [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) eigenschap binnen de [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview) gebruiken.

## Onderhoud en verlengingen

Dertig dagen voordat uw certificaat van de eerste partij verloopt, controleert de Adobe of CNAME nog geldig en in gebruik is. Als dat het geval is, gaat de Adobe ervan uit dat u de service wilt blijven gebruiken en wordt het certificaat automatisch namens u vernieuwd.

>[!IMPORTANT]
>
>Als de CNAME-record van uw organisatie wordt verwijderd of niet langer wordt toegewezen aan de opgegeven veilige hostnaam voor Adobe, kan de Adobe het certificaat niet vernieuwen. De vermelding in het systeem van de Adobe wordt gemarkeerd voor verwijdering zonder verdere communicatie.

## Veelgestelde vragen

+++Is dit proces veilig?

Ja. Het Adobe-beheerde certificaatprogramma is veiliger dan uw organisatie die Adobe van een certificaat verstrekt. Geen enkel certificaat of een persoonlijke sleutel wijzigt de handen buiten de Adobe en de certificeringsinstantie die het certificaat afgeeft.

+++

+++Hoe kan de Adobe een certificaat voor ons domein kopen?

Het certificaat kan alleen worden aangeschaft als u de opgegeven hostnaam hebt toegewezen aan een hostnaam die eigendom is van de Adobe. U delegeert deze hostname in wezen aan Adobe en staat Adobe toe om het certificaat namens u aan te schaffen.

+++

+++Kan ik verzoeken om intrekking van het certificaat?

Ja. Als eigenaar van het domein hebt u het recht om te verzoeken dat het certificaat wordt ingetrokken. Neem contact op met de klantenservice van de Adobe om dit proces te starten.

+++

+++Welk encryptietype wordt gebruikt?

Adobe werkt met DigiCert voor het uitgeven van een SHA-2-certificaat.

+++

+++Leidt dit programma tot extra kosten?

Nee. Adobe biedt deze service zonder extra kosten aan alle Adobe Experience Cloud-klanten aan.

+++

+++Welke basisveiligheidsniveaus biedt Adobe aan?

De Adobe biedt twee niveaus van de neerzetveiligheid aan om aan verschillende klantenbehoeften voor veiligheid op de inzameling van eerstepartijgegevens te voldoen. Deze niveaus bepalen welke encryptiealgoritmen voor verbindingen HTTPS met de servers van de Adobe worden gesteund. De Adobe herziet en werkt regelmatig de reeks gesteunde algoritmen bij die op huidige veiligheidspraktijken worden gebaseerd. Neem contact op met de klantenservice als u de beveiligingsinstellingen van de ontvanger wilt wijzigen.

* **Standaard** vereist TLS 1.2 of hoger en minimaal 128-bits codering. Het is ontworpen om de breedste apparaatcompatibiliteit te bieden en tegelijkertijd een veilige codering te behouden.
* **Hoog** Voor cijferbeveiligingsniveau is TLS 1.2 of hoger vereist en wordt ondersteuning voor zwakkere ciphers verwijderd. Het is ontworpen voor klanten die de sterkste encryptie willen en zich niet zorgen maken over steun voor oudere apparaten.

Van de volgende clients is bekend dat ze geen verbinding kunnen maken met de beveiliging van het script ingesteld op **Hoog**:

* Windows 8.1 en eerder (laatst bijgewerkt in 2018)
* Windows Phone 8.1 en eerder (laatst bijgewerkt in 2016)
* OS X 10.10 en eerder (laatst bijgewerkt in 2017)
* iOS 8.4 en eerder (laatstelijk bijgewerkt in 2015)

+++

+++Welke HTTPS-certificaattypen worden ondersteund?

De Adobe steunt zowel RSA als ECC certificaattypes om aan verschillende klantenbehoeften te voldoen. RSA-certificaten worden meer ondersteund voor clients, maar ECC-certificaten gebruiken minder verwerking aan zowel de server- als de clientzijde. Voor Adobe-beheerde certificaten, zowel RSA als ECC worden verstrekt. Voor klant-beheerde certificaten, zowel worden RSA als ECC geadviseerd. Moderne clients ondersteunen zowel RSA als ECC. De volgende cliënten steunen typisch slechts certificaten RSA:

* Windows Vista en eerder (laatst bijgewerkt in 2012)
* Windows Phone 8.0 en eerder (laatst bijgewerkt in 2014)
* OS X 10.8 en eerder (laatst bijgewerkt in 2013)
* iOS 5.1 en eerder (laatstelijk bijgewerkt in 2012)
* Android 4.3 en eerder (laatstelijk bijgewerkt in 2013)

+++
