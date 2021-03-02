---
description: Leer hoe Adobe Analytics cookies gebruikt om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies.
keywords: cookies;privacy
solution: Experience Cloud,Analytics
title: '"First-party cookies "'
index: y
snippet: y
feature: Cookies
topic: Beheer
role: Beheerder
level: Ervaren
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---


# Cookies van eerste bedrijven

Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies. Deze onschadelijke cookies, die afkomstig zijn uit een domein dat wordt gehost door Adobe, worden cookies van derden genoemd.

Veel browsers en anti-spywaretoepassingen zijn ontworpen om cookies van derden af te wijzen en te verwijderen, inclusief de cookies die worden gebruikt in de gegevensverzameling Analytics. Ter ondersteuning van het bijhouden van de interactie tussen uw bezoekers en uw website, kunt u cookies van de eerste fabrikant implementeren.

Er zijn twee opties beschikbaar voor het implementeren van cookies van de eerste fabrikant:

* De Experience Platform-id-service. De id-service kan het cookie in de context van de eerste partij instellen met JavaScript.
* DNS ingangen op DNS server van uw bedrijf om een alias CNAME aan een Adobe ontvangen domein te vormen. Gelieve te merken op dat terwijl diverse producten van Adobe gebruikend een CNAME steunen, in alle gevallen CNAME wordt gebruikt om tot een vertrouwd op eerste-partijeindpunt voor een specifieke klant te leiden en door die klant wordt bezeten. Als die klant veelvoudige domeinen controleert, kunnen zij één enkel eindpunt CNAME gebruiken om gebruikers over hun domeinen te volgen, maar aangezien dit derdekoekjes voor alle domeinen buiten het domein van CNAME vereist, werkt het niet wanneer derdekoekjes worden geblokkeerd en zo niet geadviseerd. Adobe CNAMEs wordt nooit gebruikt om een individu of een apparaat over domeinen te volgen die door verschillende klanten worden bezeten.

Zelfs als de eerste optie wordt gebruikt met de Experience Cloud ID-service, zal de ITP van Apple de cookies van de eerste partij van korte duur maken, zodat deze het beste samen met de tweede optie kunnen worden gebruikt.

Als uw site beveiligde pagina&#39;s heeft via het HTTPS-protocol, kunt u voor de tweede optie met een CNAME een SSL-certificaat aanvragen om cookies van de eerste partij te implementeren. Adobe raadt sterk aan dat u uitsluitend HTTPS gebruikt voor gegevensverzameling, aangezien de ondersteuning voor HTTP-verzameling in de tweede helft van 2020 afneemt.

Het SSL-certificaatuitgifteproces kan vaak verwarrend en tijdrovend zijn. Als gevolg hiervan heeft Adobe een partnerschap opgezet met DigiCert, een toonaangevende certificeringsinstantie (CA) in de industrie, en een geïntegreerd proces ontwikkeld waarmee de aankoop en het beheer van deze certificaten worden geautomatiseerd.

Met uw toestemming, zullen wij met onze CA werken om een nieuw SSL certificaat van SHA-2 voor u uit te geven, op te stellen en te beheren. Adobe blijft dit certificaat beheren en zorgt ervoor dat een onverwachte vervaldatum, intrekking of bezorgdheid over de beveiliging geen bedreiging vormt voor de beschikbaarheid van de beveiligde verzameling van uw organisatie.

## Adobe Beheerd certificaatprogramma

Het door Adobe beheerde certificaatprogramma is het aanbevolen proces voor het implementeren van een nieuw eersteklas SSL-certificaat voor cookies van de eerste fabrikant.

Met het Adobe Managed Certificate-programma kunt u zonder extra kosten een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeren (voor uw eerste 100 CNAME&#39;s). Als u momenteel uw eigen door de klant beheerde SSL-certificaat hebt, spreekt u dan met de klantenservice van Adobe over de migratie naar het door Adobe beheerde certificaatprogramma.

### Implementeren

Hieronder wordt beschreven hoe u een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeert:

1. Vul het [First-party de verzoekformulier van het koekjesverzoek](/help/interface/cookies/assets/FPC_Request_Form.xlsx) in en open een kaartje met de Zorg van de Klant die om opstelling verzoekt eerste-partijkoekjes op het Adobe Beheerde programma. Elk veld wordt in het document met voorbeelden beschreven.

1. CNAME-records maken (zie onderstaande instructies).

   Op het ontvangen van het kaartje, zou een vertegenwoordiger van de klantenzorg u van een paar verslagen van CNAME moeten voorzien. Deze verslagen moeten op DNS server van uw bedrijf worden gevormd alvorens Adobe het certificaat namens u kan kopen. De CNAMES zullen gelijkaardig aan het volgende zijn:

   **Beveiligen**  - De hostnaam  `smetrics.example.com` verwijst bijvoorbeeld naar:  `example.com.ssl.d1.omtrdc.net`.

   **Niet-beveiligd**  - De hostnaam  `metrics.example.com` verwijst bijvoorbeeld naar:  `example.com.d1.omtrdc.net`.

1. Als deze CNAMES zijn geïnstalleerd, werkt Adobe samen met DigiCert aan de aanschaf en installatie van een certificaat op Adobe productieservers.

   Als u een bestaande implementatie hebt, kunt u bezoekersmigratie overwegen om uw bestaande bezoekers te onderhouden. Nadat het certificaat live naar de productieomgeving van Adobe is geduwd, kunt u de volgende servervariabelen aan nieuwe hostnames bijwerken. Betekenis: als de site niet veilig is (HTTP), werkt u `s.trackingServer` bij. Als de site beveiligd is (HTTPS), werkt u zowel `s.trackingServer` als `s.trackingServerSecure` variabelen bij.

1. [Bevestig hostname door:sturen](#validate)  (zie hieronder).

1. [Implementatiecode](#update)  bijwerken (zie hieronder).

### Onderhoud en verlenging

SSL-certificaten verlopen elk jaar, wat betekent dat Adobe jaarlijks een nieuw certificaat voor elke implementatie moet aanschaffen. Alle ondersteunde gebruikers binnen uw organisatie ontvangen een e-mailmelding wanneer een implementatie bijna is verlopen. Om uw hostnaam te vernieuwen door Adobe, moet één ondersteunde gebruiker het e-mailbericht van Adobe beantwoorden en aangeven dat u de vervallende hostnaam voor gegevensverzameling wilt blijven gebruiken. Op dat moment koopt en installeert Adobe automatisch een nieuw certificaat.

### Veelgestelde vragen

| Vraag | Antwoord |
|---|---|
| **Is dit proces veilig?** | Ja, het Adobe Managed-programma is veiliger dan onze oudere methode, omdat geen enkel certificaat of een persoonlijke sleutel buiten de Adobe en de uitgevende certificeringsinstantie in handen verandert. |
| **Hoe kan Adobe een certificaat voor ons domein aanschaffen?** | Het certificaat kan alleen worden aangeschaft als u de opgegeven hostnaam (bijvoorbeeld `smetrics.example.com`) hebt toegewezen aan een hostnaam in eigendom van Adobe. Dit is hoofdzakelijk het delegeren van deze hostname aan Adobe en staat Adobe toe om het certificaat namens uw naam te kopen. |
| **Mag ik vragen dat het certificaat wordt ingetrokken?** | Ja, als eigenaar van het domein hebt u het recht om te vragen dat het certificaat is ingetrokken. U hoeft alleen een ticket te openen met de klantenservice om dit te laten voltooien. |
| **Gebruikt dit certificaat SHA-2-versleuteling?** | Ja, Adobe werkt met DigiCert voor het uitgeven van een SHA-2-certificaat. |
| **Betekent dit extra kosten?** | Nee, Adobe biedt deze service zonder extra kosten aan alle huidige Adobe Digital Experience-klanten. |

## CNAME-records maken

Het team van netwerkbewerkingen van uw organisatie moet uw DNS-servers configureren door nieuwe CNAME-records te maken. Elke hostname door:sturen gegevens aan de servers van de Adobe gegevensinzameling.

De specialist FPC voorziet u van gevormde hostnames en welke CNAMEs zij moeten worden gericht aan. Bijvoorbeeld:

* **SSL-hostnaam**:`smetrics.mysite.com`
* **SSL-CNAME**:`mysite.com.ssl.sc.omtrdc.net`
* **Hostnaam** niet-SSL:`metrics.mysite.com`
* **Niet-SSL CNAME**:`mysite.com.sc.omtrdc.net`

Zolang de implementatiecode niet wordt gewijzigd, heeft deze stap geen invloed op de gegevensverzameling en kan deze op elk moment na het bijwerken van de implementatiecode worden uitgevoerd.

>[!NOTE]
>
>De dienst van identiteitskaart van de Bezoeker van Experience Cloud verstrekt een alternatief aan het vormen van een NAAM om eerderekookies toe te laten, maar wegens recente veranderingen van Apple ITP, wordt het nog geadviseerd om een NAAM toe te wijzen zelfs wanneer het gebruiken van de Dienst van identiteitskaart van Experience Cloud.

## Door:sturen van hostnaam valideren {#validate}

De volgende methoden zijn beschikbaar voor validatie:

### Valideren met een browser

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, kunt u de browser gebruiken voor validatie:

`https://sstats.adobe.com/_check`

>[!NOTE]
>
>Er verschijnt een beveiligingswaarschuwing als een certificaat niet is geïnstalleerd.

### Valideren met [!DNL curl]

Adobe raadt u aan [[!DNL curl]](https://curl.haxx.se/) vanaf de opdrachtregel te gebruiken. ([!DNL Windows] gebruikers kunnen [!DNL curl] installeren van: <https://curl.haxx.se/windows/>)

Als u een CNAME hebt maar geen certificaat is geïnstalleerd, voert u het volgende uit:
`curl -k https://sstats.adobe.com/_check`
Reactie: `SUCCESS`

(De waarde `-k` schakelt de beveiligingswaarschuwing uit.)

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, voert u het volgende uit:
`curl https://sstats.adobe.com/_check`
Reactie: `SUCCESS`

### Valideren met [!DNL nslookup]

U kunt `nslookup` voor bevestiging gebruiken. Als voorbeeld gebruikt `sstats.adobe.com`open een bevelherinnering en type `nslookup sstats.adobe.com`

Als alles goed is ingesteld, ziet u een resultaat dat vergelijkbaar is met:

```
nslookup sstats.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

sstats.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## Implementatiecode {#update} bijwerken

Voordat u code op uw site bewerkt om cookies van andere bedrijven te gebruiken, moet u aan de volgende voorwaarden voldoen:

* Vraag een SSL-certificaat aan door de stappen uit te voeren die hierboven zijn beschreven in de sectie *Implementeren* van het [Beheerde certificaatprogramma voor Adobe](#adobe-managed-certificate-program).
* CNAME-records maken (zie hierboven).
* Valideer de hostnaam of -namen (zie boven).

Nadat u hebt gecontroleerd uw hostname(en) antwoorden en door:sturen aan de servers van de gegevensinzameling van de Adobe, kunt u uw implementatie veranderen om aan uw eigen server van de gegevensinzameling te richten hostnames.

1. Open uw kernJavaScript dossier (`s_code.js/AppMeasurement.js`).
1. Als u de codeversie wilt bijwerken, vervangt u het gehele `s_code.js/AppMeasurement.js`-bestand door de nieuwere versie en vervangt u eventuele plug-ins of aanpassingen. **Of**, als u de code wilt bijwerken slechts relevant aan eerderangs koekjes, bepaal de plaats van s.trackingServer en s.trackingServerSecure (als het gebruiken van SSL) variabelen, en richt hen aan uw nieuwe hostnames van de gegevensinzameling. Het gebruiken van mysite.com als voorbeeld:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Upload het bijgewerkte kern-JavaScript-bestand naar uw site.

1. Als u naar eersteklas koekjes van een reeds lang bestaande implementatie, of het veranderen in een verschillende eerste-partijinzameling hostname beweegt, adviseren wij migrerende bezoekers van het vorige domein aan het nieuwe domein.

Zie [Migratie van bezoekers](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) in de handleiding voor analytische implementatie.

Nadat u het JavaScript-bestand hebt geüpload, wordt alles geconfigureerd voor de verzameling van cookie van de eerste partij. Wij adviseren dat u Analytics het melden voor de volgende verscheidene uren controleert om ervoor te zorgen dat de gegevensinzameling zoals normaal verdergaat. Als dit niet het geval is, controleert u of alle bovenstaande stappen zijn uitgevoerd en laat een van de ondersteunde gebruikers van uw organisatie contact opnemen met de klantenservice.
