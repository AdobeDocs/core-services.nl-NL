---
description: Leer hoe Adobe Analytics cookies gebruikt om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies.
keywords: cookies;privacy
solution: Experience Cloud,Analytics
title: '"First-party cookies "'
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 00a6aa791dd08c2907cd09c17b7e2a1e62b060c1
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 0%

---

# Cookies van eerste bedrijven

Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies. Waar mogelijk gebruikt Adobe cookies van de eerste partij om activiteiten op uw site op te nemen. Als u activiteit wilt opnemen op verschillende sites, zoals andere domeinen die u hebt, zijn cookies van andere bedrijven vereist.

Veel browsers en antispywaretoepassingen zijn ontworpen om cookies van derden af te wijzen en te verwijderen. Adobe zorgt ervoor dat cookies altijd kunnen worden ingesteld, zelfs als cookies van derden worden geblokkeerd. Het specifieke gedrag varieert afhankelijk van of u de Dienst van de Identiteit van het Experience Platform (de Dienst van ECID) of de erfenisherkenningstekens van Analytics (ook bekend als s_vi koekje) gebruikt:

* De [Experience Platform Identity Service (ECID Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=en) automatisch cookies van eerste bedrijven instellen, ongeacht of uw verzamelingsdomein overeenkomt met uw sitedomein. Als deze niet overeenkomen, gebruikt de Identity Service JavaScript om cookies in te stellen in het domein van uw site.
* Als u [Verouderde id&#39;s analyseren](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-analytics.html?lang=en) (ook bekend als de `s_vi` cookie) het is afhankelijk van de configuratie van uw gegevensverzamelingsserver. Als de server van de gegevensinzameling het domein van uw plaats aanpast, dan worden de koekjes geplaatst als eerste-partij. Als de verzamelingsserver niet overeenkomt met uw huidige domein, worden cookies ingesteld als derden. In dit geval stelt Analytics een first-party-cookies in als cookies van derden worden geblokkeerd [fallback-id (s_fid)](cookies-analytics.md) in plaats van de standaard &#39;s_vi&#39; cookie.

Als u uw inzamelingsserver zou willen verzekeren past uw domein van de plaats aan, kunt u een implementatie gebruiken CNAME die het door:sturen van een douanedomein zal toelaten dat in uw implementatie CNAME aan de inzamelingsservers van Adobe wordt gespecificeerd. Dit impliceert veranderingen in DNS van uw bedrijf montages om een alias van CNAME aan het richten aan een Adobe ontvangen domein te vormen. Gelieve te merken op dat terwijl diverse producten van Adobe gebruikend een CNAME steunen, in alle gevallen CNAME wordt gebruikt om tot een vertrouwd op eerste-partijeindpunt voor een specifieke klant te leiden en door die klant wordt bezeten. Als u veelvoudige domeinen controleert, kunnen zij één enkel eindpunt CNAME gebruiken om gebruikers over hun domeinen te volgen, maar waar het plaatsdomein niet de het domeinkoekjes van CNAME aanpast wordt geplaatst als derde.

>[!NOTE]
>
>Ongeacht of uw inzamelingsdomein uw plaatsdomein aanpast, maakt het Programma van de Preventie van het Intelligente Volgen van Apple (ITP) de eerste partijkoekjes die door Adobe worden geplaatst kortstondig op browsers die door ITP worden geregeerd, die Safari op macOS en alle browsers op iOS en iPadOS omvatten. Vanaf november 2020 hebben cookies die via CNAME zijn ingesteld, dezelfde vervaldatum als cookies die via JavaScript zijn ingesteld. Deze vervaldatum kan worden gewijzigd.

Als u een NAAM voor gegevensinzameling wilt vestigen en als uw plaats veilige pagina&#39;s gebruikend het protocol HTTPS heeft, kunt u met Adobe werken om een SSL certificaat te verkrijgen.

Het SSL-certificaatuitgifteproces kan vaak verwarrend en tijdrovend zijn. Als gevolg hiervan heeft Adobe een partnerschap opgezet met DigiCert, een toonaangevende certificeringsinstantie (CA), en een geïntegreerd proces ontwikkeld waarmee de aankoop en het beheer van deze certificaten worden geautomatiseerd.

Met uw toestemming, werken wij met CA om, een nieuw SSL certificaat van SHA-2 voor u uit te geven op te stellen en te beheren. Adobe blijft dit certificaat beheren en zorgt ervoor dat een onverwachte vervaldatum, intrekking of bezorgdheid over de beveiliging geen bedreiging vormt voor de beschikbaarheid van de beveiligde verzameling van uw organisatie.

## Adobe-Beheerd certificaatprogramma

Het Adobe Beheerde Programma van het Certificaat is het geadviseerde proces voor vestiging het eerste-partijSSL certificaat nodig voor een implementatie CNAME die ervoor zorgt uw de inzamelingsserver van de Adobe uw plaatsdomein aanpast.

Met het Adobe Managed Certificate-programma kunt u zonder extra kosten een nieuw SSL-certificaat van de eerste partij implementeren (voor uw eerste 100 CNAME&#39;s). Als u momenteel uw eigen door de klant beheerde SSL-certificaat hebt, spreekt u dan met de klantenservice van Adobe over de migratie naar het door Adobe beheerde certificaatprogramma.

### Implementeren

Hier is hoe u een nieuw eerste-partijSSL certificaat voor de inzameling van eerste-partijgegevens uitvoert:

1. Vul de [Formulier voor eerste domeinaanvraag](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) en een ticket te openen met de klantenservice, waarbij de eerste-partij gegevensverzameling wordt gevraagd voor het door Adobe beheerde programma. Elk veld wordt in het document met voorbeelden beschreven.

2. CNAME-records maken (zie onderstaande instructies).

   Na het ontvangen van het kaartje, zou een vertegenwoordiger van de klantenzorg u van een verslag CNAME moeten voorzien. Deze verslagen moeten op DNS server van uw bedrijf worden gevormd alvorens Adobe het certificaat namens u kan kopen. De CNAME is gelijkaardig aan het volgende:

   **Beveiligen** - Bijvoorbeeld de hostnaam `smetrics.example.com` punten naar: `example.com.adobedc.net`.

>[!NOTE]
> In het verleden, adviseerde Adobe dat klanten twee CNAME, voor HTTPS en één voor HTTP instellen. Aangezien het beste praktijken is om verkeer te coderen en de meeste browsers sterk ontmoedigen HTTP, adviseren wij niet meer vestiging een NAAM voor HTTP. Neem contact op met de klantenservice van Adobe om uw CNAME voor HTTP te configureren.

1. Als de CNAME is geactiveerd, werkt Adobe samen met DigiCert aan de aanschaf en installatie van een certificaat op productieservers van Adobe.

   Als u een bestaande implementatie hebt, kunt u bezoekersmigratie overwegen om uw bestaande bezoekers te onderhouden. Nadat het certificaat live naar de productieomgeving van Adobe is geduwd, kunt u de volgende servervariabelen aan nieuwe hostnames bijwerken. Betekenis: als de site niet veilig is (HTTP), werkt u de `s.trackingServer`. Als de site beveiligd is (HTTPS), werkt u beide bij `s.trackingServer` en `s.trackingServerSecure` variabelen.

2. [Hostnaam doorsturen valideren](#validate) (zie hieronder).

3. [Implementatiecode bijwerken](#update) (zie hieronder).

### Onderhoud en verlenging

SSL-certificaten verlopen elk jaar, wat betekent dat Adobe jaarlijks een nieuw certificaat voor elke implementatie moet aanschaffen. Alle ondersteunde gebruikers binnen uw organisatie ontvangen een e-mailmelding wanneer een implementatie bijna is verlopen. Om uw hostnaam te vernieuwen door Adobe, moet één ondersteunde gebruiker het e-mailbericht van Adobe beantwoorden en aangeven dat u de vervallende hostnaam voor gegevensverzameling wilt blijven gebruiken. Op dat moment koopt en installeert Adobe automatisch een nieuw certificaat.

### Veelgestelde vragen

| Vraag | Antwoord |
|---|---|
| **Is dit proces veilig?** | Ja, het Adobe-Beheerde programma is veiliger dan onze oudere methode aangezien geen certificaat of privé sleutel buiten Adobe en de uitgevende certificaatautoriteit van handen verandert. |
| **Hoe kan Adobe een certificaat voor ons domein aanschaffen?** | Het certificaat kan alleen worden aangeschaft als u de opgegeven hostnaam hebt opgegeven (bijvoorbeeld `telemetry.example.com`) aan een hostnaam in eigendom van Adobe. Dit is hoofdzakelijk het delegeren van deze hostname aan Adobe en staat Adobe toe om het certificaat namens uw naam te kopen. |
| **Mag ik vragen dat het certificaat wordt ingetrokken?** | Ja, als eigenaar van het domein hebt u het recht om te verzoeken dat het certificaat wordt ingetrokken. Open een ticket met de klantenservice om dit te laten voltooien. |
| **Gebruikt dit certificaat SHA-2-versleuteling?** | Ja, Adobe werkt met DigiCert voor het uitgeven van een SHA-2-certificaat. |
| **Betekent dit extra kosten?** | Nee, Adobe biedt deze service zonder extra kosten aan alle huidige Adobe Digital Experience-klanten. |

{style=&quot;table-layout:auto&quot;}

## CNAME-records maken

Het team van netwerkbewerkingen van uw organisatie moet uw DNS-servers configureren door CNAME-records te maken. Elke hostname door:sturen gegevens aan de servers van de Adobe gegevensinzameling.

De specialist FPC voorziet u van gevormde hostname en welke CNAME zij moeten worden gericht aan. Bijvoorbeeld:

* **SSL-hostnaam**:`smetrics.mysite.com`
* **SSL CNAME**:`mysite.com.adobedc.net`

>[!NOTE]
> Als u nog steeds onveilig gebruikt, ziet het er als volgt uit:
> * **Hostnaam niet-SSL**:`metrics.mysite.com`
> * **Niet-SSL CNAME**:`mysite.com.adobedc.net`


Zolang de implementatiecode niet wordt gewijzigd, heeft deze stap geen invloed op de gegevensverzameling en kan deze op elk moment na het bijwerken van de implementatiecode worden uitgevoerd.

## Hostnaam doorsturen valideren {#validate}

De volgende methoden zijn beschikbaar voor validatie:

### Valideren met een browser

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, kunt u de browser gebruiken voor validatie:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Er wordt een beveiligingswaarschuwing weergegeven als een certificaat niet is geïnstalleerd.

### Valideren met [!DNL curl]

Adobe raadt u aan [[!DNL curl]](https://curl.se/) vanaf de opdrachtregel. ([!DNL Windows] gebruikers kunnen installeren [!DNL curl] van: <https://curl.se/windows/>)

Als u een CNAME hebt maar geen certificaat is geïnstalleerd, voert u het volgende uit:
`curl -k https://smetrics.adobe.com/_check`
Reactie: `SUCCESS`

(De `-k` waarde schakelt de beveiligingswaarschuwing uit.)

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, voert u het volgende uit:
`curl https://smetrics.adobe.com/_check`
Reactie: `SUCCESS`

### Valideren met [!DNL nslookup]

U kunt `nslookup` voor validatie. Gebruiken `smetrics.adobe.com`als voorbeeld, open een bevelherinnering en type `nslookup smetrics.adobe.com`

Als alles met succes opstelling is, ziet u een terugkeer gelijkend op:

```
nslookup smetrics.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

smetrics.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## Implementatiecode bijwerken {#update}

Alvorens u code op uw plaats uitgeeft om de inzameling van de eerste partijgegevens te gebruiken, voltooi deze eerste vereisten:

* Vraag een SSL-certificaat aan door de hierboven beschreven stappen in het dialoogvenster *Implementeren* van de [Adobe-Beheerd certificaatprogramma](#adobe-managed-certificate-program).
* CNAME-records maken (zie hierboven).
* Valideer de hostnamen (zie hierboven).

Nadat u hebt geverifieerd uw hostnames antwoorden en aan de servers van de Adobe gegevensinzameling door:sturen, kunt u uw implementatie veranderen om aan uw eigen server van de gegevensinzameling te richten hostnames.

1. Uw kern-JavaScript-bestand openen (`s_code.js/AppMeasurement.js`).
1. Als u de versie van de code wilt bijwerken, vervangt u de volledige code `s_code.js/AppMeasurement.js` met de nieuwere versie te openen en eventuele plug-ins of aanpassingen te vervangen. **of**, als u de code wilt bijwerken slechts relevant aan de inzameling van eerste-partijgegevens, bepaal de plaats van s.trackingServer en s.trackingServerSecure (als het gebruiken van SSL) variabelen, en richt hen aan uw nieuwe servers van de gegevensinzameling. Mijn site.com gebruiken als voorbeeld:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Upload het bijgewerkte kern-JavaScript-bestand naar uw site.

1. Als u zich aan de inzameling van de eerste-partijgegevens van een reeds lang bestaande implementatie beweegt, of het veranderen in een verschillende eerste-partijinzameling hostname, adviseert Adobe migrerende bezoekers van het vorige domein aan het nieuwe domein.

Zie [Migratie bezoeker](https://experienceleague.adobe.com/docs/analytics/technotes/visitor-migration.html?lang=en) in de handleiding voor analytische implementatie.

Nadat u het JavaScript-bestand hebt geüpload, wordt alles geconfigureerd voor gegevensverzameling van de eerste partij. Adobe raadt u aan de analytische rapportage de komende uren te controleren om ervoor te zorgen dat de gegevensverzameling normaal blijft. Als dit niet het geval is, controleert u of alle bovenstaande stappen zijn uitgevoerd en laat een van de ondersteunde gebruikers van uw organisatie contact opnemen met de klantenservice.
