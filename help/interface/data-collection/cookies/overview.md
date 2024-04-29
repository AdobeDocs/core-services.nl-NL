---
description: Leer hoe oplossingen en services in Adobe Experience Cloud cookies gebruiken.
title: Hoe cookies worden gebruikt in Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '890'
ht-degree: 0%

---


# In Experience Cloud gebruikte cookies

Veel services in de Adobe Experience Cloud gebruiken cookies. Een cookie is een klein stukje gegevens dat door een website aan een webbrowser wordt gepresenteerd. De browser slaat dit stukje gegevens op, zodat een website zo nodig naar de gegevens kan verwijzen. Deze handeling wordt uitgevoerd bij elke volgende aanvraag voor pagina&#39;s en afbeeldingen.

Er worden cookies geleverd om tijdens en soms tussen bezoeken aan een website informatie te bewaren. Met cookies kunnen apparaten op unieke wijze worden onderscheiden van andere browsers die de site weergeven.

De wetten, de verordeningen, en de zelfreguleringsprincipes vereisen u om toestemming van bezoekers te verkrijgen alvorens u informatie op een computer of een ander Web verbonden apparaat kunt opslaan of terugwinnen. Adobe stelt voor dat u met de juridische adviseur van uw organisatie controleert welke wetten, regels, en principes uw gebruik van koekjes controleren.

## Cookies van eerste bedrijven

Adobe Experience Cloud-services gebruiken cookies om informatie te verschaffen over variabelen en componenten die niet aanwezig zijn tussen afbeeldingsaanvragen en browsersessies. Waar mogelijk gebruikt de Adobe cookies van de eerste partij om activiteiten op uw site op te nemen. Als u activiteit wilt opnemen op verschillende sites, zoals andere domeinen die u hebt, zijn cookies van andere bedrijven vereist.

Veel browsers en antispywaretoepassingen zijn ontworpen om cookies van derden af te wijzen en te verwijderen. Adobe zorgt ervoor dat cookies altijd kunnen worden ingesteld, zelfs als cookies van derden worden geblokkeerd. Het specifieke gedrag varieert afhankelijk van of u de Dienst van de Identiteit van het Experience Platform (de Dienst van ECID) of de erfenisherkenningstekens van Analytics (zoals gebruikt `s_vi` cookie):

* De [Experience Platform Identity Service (ECID Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) plaatst automatisch eerste-partijkoekjes ongeacht of uw inzamelingsdomein uw plaatsdomein aanpast. Als deze niet overeenkomen, gebruikt de identiteitsservice JavaScript om cookies in te stellen op het domein van uw site.
* Als u [Verouderde id&#39;s analyseren](analytics.md) (zoals de `s_vi` cookie), is het afhankelijk van de configuratie van uw gegevensverzamelingsserver. Als de server van de gegevensinzameling het domein van uw plaats aanpast, dan worden de koekjes geplaatst als eerste-partij. Als de verzamelingsserver niet overeenkomt met uw huidige domein, worden cookies ingesteld als derde. Als cookies van derden in dit geval worden geblokkeerd, stelt Analytics een fallback-id van de eerste partij in (`s_fid`) in plaats van de norm `s_vi` cookie.

Als u zou willen ervoor zorgen dat uw inzamelingsserver het domein van uw plaats aanpast, kunt u een implementatie gebruiken CNAME die het door:sturen van een douanedomein toelaat dat in uw implementatie CNAME aan de inzamelingsservers van de Adobe wordt gespecificeerd. Deze taak impliceert veranderingen in DNS montages van uw bedrijf om een alias van CNAME aan het richten aan een Adobe ontvangen domein te vormen. Gelieve te merken op dat terwijl diverse producten van de Adobe het gebruiken van een CNAME steunen, in alle gevallen CNAME wordt gebruikt om tot een vertrouwd op eerste-partijeindpunt voor een specifieke klant te leiden en door die klant wordt bezeten. Als u veelvoudige domeinen controleert, kunnen zij één enkel eindpunt CNAME gebruiken om gebruikers over hun domeinen te volgen, maar waar het plaatsdomein niet de het domeinkoekjes van CNAME aanpast worden geplaatst als derde.

>[!NOTE]
>
>Ongeacht of uw inzamelingsdomein uw plaatsdomein aanpast, maakt het programma van de Preventie van het Intelligente Volgen van de Apple (ITP) de eerste partijkoekjes door Adobe worden geplaatst kortstondig op browsers die door ITP worden geregeerd, die Safari op macOS en alle browsers op iOS en iPadOS omvatten. Vanaf november 2020 hebben cookies die via CNAME zijn ingesteld, dezelfde vervaldatum als cookies die via JavaScript zijn ingesteld. Deze vervaldatum kan worden gewijzigd.

## Cookies en privacy

Het handhaven van klantenprivacy en gegevensveiligheid zijn hoogste prioriteiten bij Adobe. Adobe neemt deel aan meerdere privacyorganisaties en werkt samen met privacytoezichthouders en zelfreguleringsbeginselen. Deze samenwerking omvat het Digital Advertising Alliance AdChoices-programma om klanten informatie te verschaffen over hoe hun informatie wordt gebruikt en over het gebruik ervan.

De meeste cookies die door Experiencen Cloud worden ingesteld, bevatten geen persoonlijk identificeerbare informatie. Deze cookies en bijbehorende gegevens zijn beveiligd en worden alleen gebruikt voor bedrijfsrapporten en voor relevante inhoud en advertenties. De gegevens zijn niet beschikbaar voor derden of andere klanten van de Adobe, tenzij ze in geaggregeerde industrieverslagen worden gebruikt. Bijvoorbeeld de [!DNL Digital Marketing Insight Report] analyseert geaggregeerde en anonieme gegevens in de detailhandel.

Adobe voegt geen browser-vlakke informatie over bedrijven samen. Om de privacy en veiligheid van de gegevens van klanten te beschermen, bieden sommige diensten binnen de Experience Cloud bedrijven de capaciteit om een afzonderlijke reeks koekjes voor elke gevolgde plaats te gebruiken. Sommige aanbiedingen bieden klanten ook de mogelijkheid om hun eigen domeinnaam als eigenaar van het cookie te gebruiken. Deze praktijk leidt tot een extra laag van privacy en veiligheid, aangezien het de koekjes van het Experience Cloud maakt *cookies van eerste partij*, permanent deel uitmaken van het terrein van de onderneming.

Cookies kunnen alleen de gegevens opslaan en verstrekken die eerder in de cookies zijn opgeslagen. Ze kunnen geen code uitvoeren of toegang krijgen tot andere informatie die op de computer is opgeslagen. Webbrowsers beperken ook de toegang tot cookiegegevens. Browsers voeren een beveiligingsbeleid voor cookies in dat alle gegevens van cookies alleen beschikbaar maakt voor de website die de informatie oorspronkelijk heeft ingesteld.

Gegevens in cookies die zijn ingesteld vanaf de website Adobe.com kunnen bijvoorbeeld niet worden bekeken door andere websites dan Adobe.com.

In het volgende diagram wordt het gebruik van cookies voor een standaardafbeeldingsaanvraag geïllustreerd:

![Koekjesgebruik voor een standaardafbeeldingsaanvraag](assets/CookiesProcessGraphic-01.png)

In het volgende diagram ziet u hoe cookie wordt gebruikt voor een verzoek om een rechte afbeelding (wordt gebruikt in scenario&#39;s waarbij een JS-bestand niet wordt geladen):

![Koekjesgebruik voor een verzoek om een rechte afbeelding](assets/CookiesProcessGraphic2.png)
