---
description: Leer hoe Adobe Analytics cookies gebruikt om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies.
keywords: cookies;privacy
solution: Experience Cloud,Analytics
title: '"First-party cookies "'
index: y
snippet: y
feature: Cookies
topic: Beheer
role: Administrator
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 11b999ef0c0d4f258e8665eb9c5bf427f5d618c4
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 0%

---

# Cookies van eerste bedrijven

Analytics gebruikt cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies. Waar mogelijk gebruikt Adobe cookies van de eerste partij om activiteiten op uw site op te nemen. Als u activiteit wilt opnemen op verschillende sites, zoals andere domeinen die u hebt, zijn cookies van andere bedrijven vereist.

Veel browsers en antispywaretoepassingen zijn ontworpen om cookies van derden af te wijzen en te verwijderen, inclusief cookies die worden gebruikt in [!DNL Analytics] gegevensverzameling. Voor ondersteuning van het bijhouden van de interactie tussen uw bezoekers en uw website moet u ervoor zorgen dat u de gegevensverzameling hebt geconfigureerd voor het gebruik van cookies van de eerste partij:

Er zijn twee opties beschikbaar voor het implementeren van cookies van de eerste fabrikant:

* Als u de Dienst van de Identiteit van het Experience Platform (de Dienst van ECID) gebruikt, plaatst het automatisch koekjes in de eerste partijcontext gebruikend JavaScript.
* Als u [!DNL Analytics] verouderde herkenningstekens (ook bekend als het `s_vi` koekje) gebruikt, hangt het af van hoe u uw server van de gegevensinzameling hebt gevormd. Als de server van de gegevensinzameling het domein van uw plaats aanpast, dan worden de koekjes geplaatst als eerste-partij. Als de verzamelingsserver niet overeenkomt met uw huidige domein, worden cookies ingesteld als derden. Als cookies van derden worden geblokkeerd, [!DNL Analytics] stelt [fallback-id (s_fid)](cookies-analytics.md) in plaats van de standaard &#39;s_vi&#39;-cookie in.

Om ervoor te zorgen dat uw verzamelingsserver overeenkomt met het domein van uw site, kunt u een CNAME-implementatie gebruiken waarmee cookies kunnen worden ingesteld in een context van een eerste partij. Dit impliceert veranderingen in DNS van uw bedrijf montages om een alias van CNAME aan het richten aan een Adobe ontvangen domein te vormen. Gelieve te merken op dat terwijl diverse producten van Adobe gebruikend een CNAME steunen, in alle gevallen CNAME wordt gebruikt om tot een vertrouwd op eerste-partijeindpunt voor een specifieke klant te leiden en door die klant wordt bezeten. Als u veelvoudige domeinen controleert, kunnen zij één enkel eindpunt CNAME gebruiken om gebruikers over hun domeinen te volgen, maar waar het plaatsdomein niet de het domeinkoekjes van CNAME aanpast wordt geplaatst als derde.

>[!NOTE]
>
>Voor beide opties maakt het ITP-programma (Intelligent Tracking Prevention) van Apple de cookies van de eerste partij van korte duur op browsers die onder ITP vallen, waaronder Safari op MacOS en alle browsers op iOS en iPadOS. Vanaf november 2020 hebben beide typen cookies een vervaldatum van zeven dagen. Deze vervaldatum kan worden gewijzigd.

Als uw site beveiligde pagina&#39;s heeft via het HTTPS-protocol, kunt u voor de tweede optie met een CNAME een SSL-certificaat aanvragen om cookies van de eerste partij te implementeren. Adobe adviseert sterk dat u exclusief HTTPS voor gegevensinzameling gebruikt aangezien Adobe steun voor HTTP- inzameling in de tweede helft van 2020 vermindert.

Het SSL-certificaatuitgifteproces kan vaak verwarrend en tijdrovend zijn. Als gevolg hiervan heeft Adobe een partnerschap opgezet met DigiCert, een toonaangevende certificeringsinstantie (CA), en een geïntegreerd proces ontwikkeld waarmee de aankoop en het beheer van deze certificaten worden geautomatiseerd.

Met uw toestemming, werken wij met CA om, een nieuw SSL certificaat van SHA-2 voor u uit te geven op te stellen en te beheren. Adobe blijft dit certificaat beheren en zorgt ervoor dat een onverwachte vervaldatum, intrekking of bezorgdheid over de beveiliging geen bedreiging vormt voor de beschikbaarheid van de beveiligde verzameling van uw organisatie.

## Adobe-Beheerd certificaatprogramma

Het door Adobe beheerde certificaatprogramma is het aanbevolen proces voor het implementeren van een nieuw eersteklas SSL-certificaat voor cookies van de eerste fabrikant.

Met het Adobe Managed Certificate-programma kunt u zonder extra kosten een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeren (voor uw eerste 100 CNAME&#39;s). Als u momenteel uw eigen door de klant beheerde SSL-certificaat hebt, spreekt u dan met de klantenservice van Adobe over de migratie naar het door Adobe beheerde certificaatprogramma.

### Implementeren

Hieronder wordt beschreven hoe u een nieuw SSL-certificaat van de eerste partij voor cookies van de eerste partij implementeert:

1. Vul het [First-party de verzoekformulier van het koekjesverzoek](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) in en open een kaartje met de Zorg van de Klant die om opstelling verzoekt eerste-partijkoekjes op het Adobe-Beheerde programma. Elk veld wordt in het document met voorbeelden beschreven.

2. CNAME-records maken (zie onderstaande instructies).

   Na het ontvangen van het kaartje, zou een vertegenwoordiger van de klantenzorg u van een verslag CNAME moeten voorzien. Deze verslagen moeten op DNS server van uw bedrijf worden gevormd alvorens Adobe het certificaat namens u kan kopen. De CNAME is gelijkaardig aan het volgende:

   **Beveiligen**  - De hostnaam  `smetrics.example.com` verwijst bijvoorbeeld naar:  `example.com.adobedc.net`.

>[!NOTE]
> In het verleden, adviseerde Adobe dat klanten twee CNAME voor HTTPS en één voor HTTP instellen. Aangezien het een beste praktijk is om verkeer te coderen en de meeste browsers sterk ontmoedigend HTTP zijn adviseren wij niet meer vestiging een NAAM voor HTTP. Indien nodig, zou het als volgt kijken:
>    **Niet-beveiligd** — de hostnaam `metrics.example.com` verwijst naar: `example.com.adobedc.net`.

1. Als de CNAME is geactiveerd, werkt Adobe samen met DigiCert aan de aanschaf en installatie van een certificaat op productieservers van Adobe.

   Als u een bestaande implementatie hebt, kunt u bezoekersmigratie overwegen om uw bestaande bezoekers te onderhouden. Nadat het certificaat live naar de productieomgeving van Adobe is geduwd, kunt u de volgende servervariabelen aan nieuwe hostnames bijwerken. Betekenis: als de site niet veilig is (HTTP), werkt u `s.trackingServer` bij. Als de site beveiligd is (HTTPS), werkt u zowel `s.trackingServer` als `s.trackingServerSecure` variabelen bij.

2. [Bevestig hostname door:sturen](#validate)  (zie hieronder).

3. [Implementatiecode](#update)  bijwerken (zie hieronder).

### Onderhoud en verlenging

SSL-certificaten verlopen elk jaar, wat betekent dat Adobe jaarlijks een nieuw certificaat voor elke implementatie moet aanschaffen. Alle ondersteunde gebruikers binnen uw organisatie ontvangen een e-mailmelding wanneer een implementatie bijna is verlopen. Om uw hostnaam te vernieuwen door Adobe, moet één ondersteunde gebruiker het e-mailbericht van Adobe beantwoorden en aangeven dat u de vervallende hostnaam voor gegevensverzameling wilt blijven gebruiken. Op dat moment koopt en installeert Adobe automatisch een nieuw certificaat.

### Veelgestelde vragen

| Vraag | Antwoord |
|---|---|
| **Is dit proces veilig?** | Ja, het Adobe-Beheerde programma is veiliger dan onze oudere methode aangezien geen certificaat of privé sleutel buiten Adobe en de uitgevende certificaatautoriteit van handen verandert. |
| **Hoe kan Adobe een certificaat voor ons domein aanschaffen?** | Het certificaat kan alleen worden aangeschaft als u de opgegeven hostnaam (bijvoorbeeld `telemetry.example.com`) hebt toegewezen aan een hostnaam in eigendom van Adobe. Dit is hoofdzakelijk het delegeren van deze hostname aan Adobe en staat Adobe toe om het certificaat namens uw naam te kopen. |
| **Mag ik vragen dat het certificaat wordt ingetrokken?** | Ja, als eigenaar van het domein hebt u het recht om te vragen dat het certificaat is ingetrokken. U hoeft alleen een ticket te openen met de klantenservice om dit te laten voltooien. |
| **Gebruikt dit certificaat SHA-2-versleuteling?** | Ja, Adobe werkt met DigiCert voor het uitgeven van een SHA-2-certificaat. |
| **Betekent dit extra kosten?** | Nee, Adobe biedt deze service zonder extra kosten aan alle huidige Adobe Digital Experience-klanten. |

## CNAME-records maken

Het team van netwerkbewerkingen van uw organisatie moet uw DNS-servers configureren door CNAME-records te maken. Elke hostname door:sturen gegevens aan de servers van de Adobe gegevensinzameling.

De specialist FPC voorziet u van gevormde hostname en welke CNAME zij moeten worden gericht aan. Bijvoorbeeld:

* **SSL-hostnaam**:`smetrics.mysite.com`
* **SSL-CNAME**:`mysite.com.adobedc.net`

>[!NOTE]
> Als u nog steeds onveilig gebruikt, ziet het er als volgt uit:
> * **Hostnaam** niet-SSL:`metrics.mysite.com`
> * **Niet-SSL CNAME**:`mysite.com.adobedc.net`


Zolang de implementatiecode niet wordt gewijzigd, heeft deze stap geen invloed op de gegevensverzameling en kan deze op elk moment na het bijwerken van de implementatiecode worden uitgevoerd.

>[!NOTE]
>
>De dienst van identiteitskaart van de Bezoeker van Experience Cloud verstrekt een alternatief aan het vormen van een CNAME om eerderangs koekjes toe te laten.

## Hostnaam doorsturen valideren {#validate}

De volgende methoden zijn beschikbaar voor validatie:

### Valideren met een browser

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, kunt u de browser gebruiken voor validatie:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Er wordt een beveiligingswaarschuwing weergegeven als een certificaat niet is geïnstalleerd.

### Valideren met [!DNL curl]

Adobe raadt u aan [[!DNL curl]](https://curl.se/) vanaf de opdrachtregel te gebruiken. ([!DNL Windows] gebruikers kunnen [!DNL curl] installeren van: <https://curl.se/windows/>)

Als u een CNAME hebt maar geen certificaat is geïnstalleerd, voert u het volgende uit:
`curl -k https://smetrics.adobe.com/_check`
Reactie: `SUCCESS`

(De waarde `-k` schakelt de beveiligingswaarschuwing uit.)

Als u een CNAME-instelling hebt en het certificaat is geïnstalleerd, voert u het volgende uit:
`curl https://smetrics.adobe.com/_check`
Reactie: `SUCCESS`

### Valideren met [!DNL nslookup]

U kunt `nslookup` voor bevestiging gebruiken. Als voorbeeld gebruikt `smetrics.adobe.com`open een bevelherinnering en type `nslookup smetrics.adobe.com`

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

Voordat u code op uw site bewerkt om cookies van andere bedrijven te gebruiken, moet u aan de volgende voorwaarden voldoen:

* Vraag een SSL-certificaat aan door de stappen hierboven beschreven in de sectie *Implementeren* van het [Door Adobe beheerde certificaatprogramma](#adobe-managed-certificate-program) uit te voeren.
* CNAME-records maken (zie hierboven).
* Valideer de hostnamen (zie hierboven).

Nadat u hebt geverifieerd uw hostnames antwoorden en aan de servers van de Adobe gegevensinzameling door:sturen, kunt u uw implementatie veranderen om aan uw eigen server van de gegevensinzameling te richten hostnames.

1. Open uw kernJavaScript dossier (`s_code.js/AppMeasurement.js`).
1. Als u de codeversie wilt bijwerken, vervangt u het gehele `s_code.js/AppMeasurement.js`-bestand door de nieuwere versie en vervangt u eventuele plug-ins of aanpassingen. **Of**, als u de code wilt bijwerken slechts relevant aan eerderangs koekjes, bepaal de plaats van s.trackingServer en s.trackingServerSecure (als het gebruiken van SSL) variabelen, en richt hen aan uw nieuwe hostnames van de gegevensinzameling. Het gebruiken van mysite.com als voorbeeld:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Upload het bijgewerkte kern-JavaScript-bestand naar uw site.

1. Als u naar de koekjes van eerste-partij van een reeds lang bestaande implementatie, of het veranderen in een verschillende eerste-partijinzameling hostname overgaat, adviseert Adobe migrerend bezoekers van het vorige domein aan het nieuwe domein.

Zie [Migratie van bezoekers](https://experienceleague.adobe.com/docs/analytics/implementation/javascript-implementation/visitor-migration.html?lang=en) in de handleiding voor analytische implementatie.

Nadat u het JavaScript-bestand hebt geüpload, wordt alles geconfigureerd voor de verzameling van cookie van de eerste partij. Adobe raadt u aan de analytische rapportage de komende uren te controleren om ervoor te zorgen dat de gegevensverzameling normaal blijft. Als dit niet het geval is, controleert u of alle bovenstaande stappen zijn uitgevoerd en laat een van de ondersteunde gebruikers van uw organisatie contact opnemen met de klantenservice.
