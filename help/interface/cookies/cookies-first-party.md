---
description: Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies.
keywords: cookies;privacy
seo-description: Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies.
seo-title: Eerste cookies
solution: Experience Cloud,Analytics
title: Eerste cookies
index: y
snippet: y
translation-type: tm+mt
source-git-commit: b6ef7f0b7ef3b43b437524b20cee940889c26ba8

---


# Cookies van eerste bedrijven

Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies. Deze onschadelijke cookies, die afkomstig zijn uit een domein dat wordt gehost door Adobe, worden cookies van derden genoemd.

Veel browsers en anti-spywaretoepassingen zijn ontworpen om cookies van derden af te wijzen en te verwijderen, inclusief de cookies die worden gebruikt in de gegevensverzameling Analytics. Ter ondersteuning van het bijhouden van de interactie tussen uw bezoekers en uw website, kunt u cookies van de eerste fabrikant implementeren.

Er zijn twee opties beschikbaar voor het implementeren van cookies van de eerste fabrikant:

* The Experience Platform ID Service. De id-service kan het cookie in de context van de eerste partij instellen met JavaScript.
* DNS-vermeldingen op de DNS-server van uw bedrijf om een CNAME-alias te configureren voor een door Adobe gehost domein. Houd er rekening mee dat diverse Adobe-producten het gebruik van een CNAME ondersteunen, maar dat de CNAME in alle gevallen wordt gebruikt om een vertrouwd primair eindpunt voor een bepaalde klant te maken en eigendom is van die klant. Als die klant veelvoudige domeinen controleert, kunnen zij één enkel eindpunt CNAME gebruiken om gebruikers over hun domeinen te volgen, maar aangezien dit derdekoekjes voor alle domeinen buiten het domein van CNAME vereist, werkt het niet wanneer derdekoekjes worden geblokkeerd en zo niet geadviseerd. Adobe CNAMEs wordt nooit gebruikt om een individu of een apparaat over domeinen te volgen die door verschillende klanten worden bezeten.

Zelfs wanneer de eerste optie wordt gebruikt met de Experience Cloud ID Service, zal de ITP van Apple de cookies van de eerste partij van korte duur maken, zodat deze het beste samen met de tweede optie wordt gebruikt.

Als uw site beveiligde pagina&#39;s heeft via het HTTPS-protocol, kunt u voor de tweede optie met een CNAME een SSL-certificaat aanvragen om cookies van de eerste fabrikant te implementeren. Adobe raadt u ten zeerste aan HTTPS uitsluitend te gebruiken voor gegevensverzameling, aangezien de ondersteuning voor HTTP-verzameling in de tweede helft van 2020 afneemt.

Het SSL-certificaatuitgifteproces kan vaak verwarrend en tijdrovend zijn. Daarom heeft Adobe een partnerschap opgezet met DigiCert, een toonaangevende certificeringsinstantie (CA), en een geïntegreerd proces ontwikkeld waarmee de aankoop en het beheer van deze certificaten worden geautomatiseerd.

Met uw toestemming, zullen wij met onze CA werken om een nieuw SSL certificaat van SHA-2 voor u uit te geven, op te stellen en te beheren. Adobe blijft dit certificaat beheren en zorgt ervoor dat een onverwachte vervaldatum, intrekking of bezorgdheid over de beveiliging de beschikbaarheid van de beveiligde verzameling van uw organisatie niet in gevaar brengt.

## Door Adobe beheerd certificaatprogramma

Het door Adobe beheerde certificaatprogramma is het aanbevolen proces voor de implementatie van een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij.

Met het Adobe Managed Certificate-programma kunt u zonder extra kosten een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeren. Als u momenteel over uw eigen door de klant beheerde SSL-certificaat beschikt, kunt u met de klantenservice van Adobe communiceren over de migratie naar het door Adobe beheerde certificaatprogramma.

### Implementeren

Hieronder wordt beschreven hoe u een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeert:

1. Vul het aanvraagformulier [voor cookies van de](/help/interface/cookies/assets/FPC_Request_Form.xlsx) eerste partij in en open een ticket met de klantenservice waarin u wordt gevraagd cookies van de eerste partij in te stellen op het door Adobe beheerde programma. Elk veld wordt in het document met voorbeelden beschreven.

1. CNAME-records maken (zie onderstaande instructies).

   Op het ontvangen van het kaartje, zou een vertegenwoordiger van de klantenzorg u van een paar verslagen van CNAME moeten voorzien. Deze records moeten op de DNS-server van uw bedrijf zijn geconfigureerd voordat Adobe het certificaat namens u kan aanschaffen. De CNAMES zullen gelijkaardig aan het volgende zijn:

   **Beveiligen** - De hostnaam verwijst bijvoorbeeld `smetrics.example.com` naar: `example.com.ssl.d1.omtrdc.net`.

   **Niet-beveiligd** - De hostnaam verwijst bijvoorbeeld `metrics.example.com` naar: `example.com.d1.omtrdc.net`.

1. Wanneer deze CNAMES zijn geïnstalleerd, werkt Adobe samen met DigiCert om een certificaat aan te schaffen en te installeren op de productieservers van Adobe.

   Als u een bestaande implementatie hebt, kunt u bezoekersmigratie overwegen om uw bestaande bezoekers te onderhouden. Nadat het certificaat live naar de productieomgeving van Adobe is geduwd, kunt u de volgservervariabelen bijwerken naar de nieuwe hostnamen. Betekenis: als de site niet veilig is (HTTP), werkt u de `s.trackingServer`. Als de site beveiligd is (HTTPS), werkt u zowel `s.trackingServer` als `s.trackingServerSecure` variabelen bij.

1. [Bevestig hostname door:sturen](#validate) (zie hieronder).

1. [Implementatiecode](#update) bijwerken (zie hieronder).

### Onderhoud en verlenging

SSL-certificaten verlopen elk jaar. Dit houdt in dat Adobe jaarlijks een nieuw certificaat voor elke implementatie moet aanschaffen. Alle ondersteunde gebruikers binnen uw organisatie ontvangen een e-mailmelding wanneer een implementatie bijna is verlopen. Adobe kan uw hostnaam alleen vernieuwen als één ondersteunde gebruiker het e-mailbericht van Adobe beantwoordt en aangeeft dat u de vervallende hostnaam voor gegevensverzameling wilt blijven gebruiken. Op dat moment koopt en installeert Adobe automatisch een nieuw certificaat.

### Veelgestelde vragen

| Vraag | Antwoord |
|---|---|
| **Is dit proces veilig?** | Ja, het Adobe Managed-programma is veiliger dan onze oude methode, omdat geen enkel certificaat of een persoonlijke sleutel buiten Adobe en de certificeringsinstantie die het certificaat uitgeeft, wordt gewijzigd. |
| **Hoe kan Adobe een certificaat voor ons domein aanschaffen?** | Het certificaat kan alleen worden aangeschaft als u de opgegeven hostnaam (bijvoorbeeld metrics.voorbeeld.com) naar een hostnaam in Adobe-eigendom hebt gestuurd. Hierdoor wordt deze hostnaam in feite gedelegeerd aan Adobe en kan Adobe het certificaat namens u aanschaffen. |
| **Mag ik vragen dat het certificaat wordt ingetrokken?** | Ja, als eigenaar van het domein hebt u het recht om te vragen dat het certificaat is ingetrokken. U hoeft alleen een ticket te openen met de klantenservice om dit te laten voltooien. |
| **Gebruikt dit certificaat SHA-2-versleuteling?** | Ja, Adobe werkt met DigiCert voor het uitgeven van een SHA-2-certificaat. |
| **Betekent dit extra kosten?** | Nee, Adobe biedt deze service zonder extra kosten aan alle huidige klanten van Adobe Digital Experience. |

## CNAME-records maken

Het team van netwerkbewerkingen van uw organisatie moet uw DNS-servers configureren door nieuwe CNAME-records te maken. Elke hostnaam stuurt gegevens door naar de gegevensverzamelingsservers van Adobe.

De specialist FPC voorziet u van gevormde hostnames en welke CNAMEs zij moeten worden gericht aan. Bijvoorbeeld:

* **SSL-hostnaam**:`smetrics.mysite.com`
* **SSL-CNAME**:`mysite.com.ssl.sc.omtrdc.net`
* **Hostnaam** niet-SSL:`metrics.mysite.com`
* **Niet-SSL CNAME**:`mysite.com.sc.omtrdc.net`

Zolang de implementatiecode niet wordt gewijzigd, heeft deze stap geen invloed op de gegevensverzameling en kan deze op elk moment na het bijwerken van de implementatiecode worden uitgevoerd.

>[!NOpmerking:]
>
>De dienst van identiteitskaart van de Bezoeker van de Wolk van de Ervaring verleent een alternatief aan het vormen van een CNAME om eerderangs koekjes toe te laten, maar wegens recente veranderingen van Apple ITP, wordt het nog geadviseerd om een CNAME toe te wijzen zelfs wanneer het gebruiken van de Dienst van identiteitskaart van de Ervaring Cloud

## Hostnaam doorsturen valideren {#validate}

De volgende methoden zijn beschikbaar voor validatie:

### Valideren met een browser

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, kunt u de browser gebruiken voor validatie:

`https://sstats.adobe.com/_check`

>[!NOpmerking:]
>
>Er verschijnt een beveiligingswaarschuwing als een certificaat niet is geïnstalleerd.

### Valideren met [!DNL curl]

Adobe raadt u aan [!DNL [curl](https://curl.haxx.se/)] vanaf de opdrachtregel te gebruiken. ([!DNL Windows] gebruikers kunnen installeren [!DNL curl] vanaf: <https://curl.haxx.se/windows/>)

Als u een CNAME hebt maar geen certificaat is geïnstalleerd, voert u het volgende uit:
`curl -k https://sstats.adobe.com/_check`Reactie: `SUCCESS`

(De `-k` waarde schakelt de beveiligingswaarschuwing uit.)

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, voert u het volgende uit:
`curl https://sstats.adobe.com/_check`Reactie: `SUCCESS`

### Valideren met [!DNL nslookup]

U kunt `nslookup` de validatie gebruiken. Als `sstats.adobe.com`voorbeeld gebruiken, open een bevelherinnering en type `nslookup sstats.adobe.com`

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

## Implementatiecode bijwerken {#update}

Voordat u code op uw site bewerkt om cookies van andere bedrijven te gebruiken, moet u aan de volgende voorwaarden voldoen:

* Vraag een SSL-certificaat aan door de hierboven beschreven stappen in de sectie *Implementeren* van het [Adobe Managed Certificate Program](#adobe-managed-certificate-program)uit te voeren.
* CNAME-records maken (zie hierboven).
* Valideer de hostnaam of -namen (zie boven).

Nadat u hebt geverifieerd dat uw hostnaam of hostnamen reageren op en doorsturen naar Adobe-servers voor gegevensverzameling, kunt u uw implementatie wijzigen en naar uw eigen hostnamen voor gegevensverzameling verwijzen.

1. Open uw kern-JavaScript-bestand (`s_code.js/AppMeasurement.js`).
1. Als u de codeversie wilt bijwerken, vervangt u het volledige `s_code.js/AppMeasurement.js` bestand door de nieuwere versie en vervangt u eventuele plug-ins of aanpassingen. **Of**, als u de code wilt bijwerken slechts relevant aan eerderangs koekjes, bepaal de plaats van s.trackingServer en s.trackingServerSecure (als het gebruiken van SSL) variabelen, en richt hen aan uw nieuwe hostnames van de gegevensinzameling. Mijn site.com gebruiken als voorbeeld:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Upload het bijgewerkte kern-JavaScript-bestand naar uw site.

1. Als u naar eersteklas koekjes van een reeds lang bestaande implementatie, of het veranderen in een verschillende eerste-partijinzameling hostname beweegt, adviseren wij migrerende bezoekers van het vorige domein aan het nieuwe domein.

Zie [Bezoekersmigratie](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) in de handleiding voor analysetoepassing.

Nadat u het JavaScript-bestand hebt geüpload, wordt alles geconfigureerd voor de verzameling van cookie van de eerste partij. Wij adviseren dat u Analytics het melden voor de volgende verscheidene uren controleert om ervoor te zorgen dat de gegevensinzameling zoals normaal verdergaat. Als dit niet het geval is, controleert u of alle bovenstaande stappen zijn uitgevoerd en laat een van de ondersteunde gebruikers van uw organisatie contact opnemen met de klantenservice.
