---
description: Leer hoe oplossingen en services in Adobe Experience Cloud cookies gebruiken.
title: Hoe cookies worden gebruikt in Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
source-git-commit: d6dc659104b3b24b60495cd97adb21ebb3962fc7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# In Experience Cloud gebruikte cookies

Adobe Experience Cloud gebruikt cookies. Een cookie is een klein stukje gegevens dat een website naar uw browser verzendt, die het opslaat voor later gebruik. Met cookies kan de website dingen onthouden wanneer u opnieuw een bezoek brengt of van pagina naar pagina gaat. Met cookies kunt u bezoeken volgen en het ene apparaat apart van het andere vertellen.

Wetten vereisen vaak dat u toestemming krijgt voordat u cookies op iemands apparaat opslaat of gebruikt. Adobe raadt u aan contact op te nemen met uw juridische team om te weten welke regels van toepassing zijn.

## Cookies van eerste bedrijven

Adobe Experience Cloud gebruikt cookies om informatie bij te houden die niet van toepassing is tussen paginaweergaven of browsersessies. Indien mogelijk gebruikt Adobe cookies van de eerste partij (gekoppeld aan uw eigen website). Voor het bijhouden van activiteiten op meerdere sites of domeinen die u bezit, zijn cookies van andere bedrijven nodig.

Sommige browsers en anti-spyware hulpmiddelen blokkeren derdekoekjes. Adobe beschikt over manieren om ervoor te zorgen dat cookies nog steeds werken, zelfs als cookies worden geblokkeerd. Hoe dit werkt, hangt af van het feit of u de Experience Platform Identity Service (ECID) of oudere Analytics-cookies (zoals het `s_vi` -cookie) gebruikt:

* [ de Dienst van de Identiteit van Experience Cloud ](https://experienceleague.adobe.com/nl/docs/id-service/using/intro/overview): De ECID Dienst plaatst altijd eerste-partijkoekjes, of uw inzamelingsdomein uw plaatsomein aanpast. Het gebruikt JavaScript om de cookie op het domein van uw site te plaatsen.

* [ Verouderde herkenningstekens van Analytics ](analytics.md) (zoals het `s_vi` koekje): Of de koekjes eerste of derde van uw opstelling afhankelijk zijn:

   * Als uw gegevensverzamelingsserver overeenkomt met het domein van uw site, zijn cookies van de eerste partij.
   * Als het niet overeenkomt, zijn cookies van derden. Als cookies van derden worden geblokkeerd, stelt Adobe een fallback-cookie (`s_fid`) in plaats van de gebruikelijke cookie.

Om ervoor te zorgen dat uw inzamelingsserver het domein van uw plaats aanpast, kunt u de opstelling van de a **NAAM** gebruiken. Hierbij moet u uw DNS-instellingen bijwerken zodat een aangepast domein (u hebt) naar Adobe-servers wordt gewijs. Hierdoor wordt de volgende cookie weergegeven als een eerderangs cookie. Terwijl één CNAME over veelvoudige domeinen kan werken, zal om het even welk domein dat niet CNAME aanpast nog derdekoekjes plaatsen.

>[!NOTE]
>
>Met Apple Intelligent Tracking Prevention (ITP) wordt de duur van Adobe-cookies van de eerste partij beperkt, zelfs als uw verzamelingsdomein overeenkomt met uw sitedomein. ITP is van invloed op Safari op macOS en op alle browsers op iOS en iPadOS. Sinds november 2020 verlopen cookies die met CNAME zijn ingesteld net zo snel als cookies die met JavaScript zijn ingesteld. Deze termijn kan in de toekomst veranderen.

Hier volgt een vereenvoudigde versie van de tekst:

## Cookies en privacy

Adobe neemt privacy en gegevensbeveiliging serieus. Het werkt met privacyorganisaties, regelgevers en programma&#39;s zoals AdChoices om mensen controle te geven over hoe hun gegevens worden gebruikt.

In de meeste cookies van Adobe Experience Cloud worden geen persoonlijke gegevens opgeslagen. Zij zijn veilig en slechts gebruikt door uw bedrijf-voor rapportering, inhoud, en reclame. Adobe deelt deze gegevens niet met andere klanten of derden, behalve in anonieme rapporten voor de hele branche (zoals Digital Marketing Insight Reports).

Adobe combineert browsergegevens niet tussen verschillende bedrijven. Om privacy te beschermen, laten sommige hulpmiddelen van Adobe elke website zijn eigen reeks koekjes gebruiken. Sommige gebruikers kunnen ook uw eigen domein voor cookies gebruiken, waardoor ze van de eerste partij een betere beveiliging krijgen.

Cookies kunnen alleen gegevens opslaan die eerder in de cookies zijn opgeslagen. Ze kunnen geen code uitvoeren of andere gegevens lezen op uw apparaat. Webbrowsers staan alleen toe dat cookies worden gelezen door de website die ze instelt. Bijvoorbeeld, slechts kan Adobe.com koekjes lezen het plaatst.

In het volgende diagram wordt het gebruik van cookies voor een standaardafbeeldingsaanvraag geïllustreerd:

![ gebruik van het Koekje voor een standaardbeeldverzoek ](assets/CookiesProcessGraphic-01.png)

In het volgende diagram ziet u hoe cookie wordt gebruikt voor een verzoek om een rechte afbeelding (wordt gebruikt in scenario&#39;s waarbij een JS-bestand niet wordt geladen):

![ gebruik van het Koekje voor een recht beeldverzoek ](assets/CookiesProcessGraphic2.png)
