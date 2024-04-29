---
description: Leer hoe Adobe Target cookies gebruikt om websitebeheerders de mogelijkheid te bieden te testen welke online inhoud en aanbiedingen voor bezoekers relevanter zijn.
solution: Target
title: Adobe Target Cookies
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 9ee4d9b0e670dec35cda530892c49e36bf7cc107
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Adobe Target cookies

Adobe Target gebruikt cookies om websitebeheerders de mogelijkheid te bieden te testen welke online-inhoud en -aanbiedingen voor bezoekers relevanter zijn.

>[!NOTE]
>
>De informatie in dit artikel is alleen van toepassing op [Adobe Target JavaScript-bibliotheek](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} (`at.js`). Zie [Adobe Experience Platform Web SDK cookies](web-sdk.md) voor informatie over de implementaties van het Doel die SDK van het Web gebruiken.
>
>U kunt de instellingen die in dit artikel worden besproken, indien nodig wijzigen, behalve voor de duur van de cookie. [Vraag uw accountvertegenwoordiger](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} bij het wijzigen van cookie-instellingen.

## Cookies van eerste bedrijven

De volgende cookies van de eerste fabrikant worden in het domein van de klant opgeslagen:

| Cookie | Details |
| --- | --- |
| `mbox` | Hiermee worden anonieme id&#39;s over de bezoeker opgeslagen.<P>**Cookie-domein**: Het domein waaruit u de mbox bedient. Omdat deze cookie wordt aangeleverd vanaf het domein van uw bedrijf, is de cookie een cookie van de eerste partij. Als een van uw domeinnamen een landcode bevat, zoals `example.co.uk`, werken met Client Services om te configureren `at.js` om deze code te ondersteunen. Voor informatie over het aanpassen van het cookiedomein, indien nodig, zie `cookieDomain` krachtens [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} in de Adobe Target-handleiding voor ontwikkelaars.<P>**Serverdomein**: `clientcode.tt.omtrdc.net`, met de clientcode voor uw Adobe Target-account.<P>**Duur van cookie**: Het cookie blijft twee jaar na de laatste aanmelding in de browser van de bezoeker staan. U kunt de duur van het cookie niet wijzigen.<P>Het cookie houdt enkele waarden bij om te beheren hoe uw bezoekers ervoeren [!DNL Target] activiteiten:<P>**sessie-id**: Een unieke id voor een bepaalde gebruikerssessie. Standaard verloopt de sessie na 30 minuten inactiviteit. Als u genereert `sessionId` uzelf (bijvoorbeeld [server-side implementaties](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), zorgt u voor het volgende:<ul><li>De sessie-id kan elke afdrukbare tekenreeks zijn, behalve een spatie, vraagteken ( ? ) of een schuine streep ( / ).</li><li>De sessie-id moet 1 tot 128 tekens lang zijn.</li><li>Voor een bepaalde sessie moet de waarde van het cookie gelijk blijven voor meerdere aanvragen.</li><li>U moet nooit parallelle sessies hebben (verschillend `sessionIds`) voor een bepaalde bezoeker op een bepaald tijdstip.</li></ul>Het verpletteren aan een bepaalde knoop in de randcluster wordt gedaan gebruikend zitting-identiteitskaart.<ul><li>De sessie is 30 minuten actief op de server. Daarom zou u geen verschillende zitting-identiteitskaart voor een bepaald moeten gebruiken `tntId/thirdPartyId` binnen 30 minuten na het laatste verzoek bij het `tntId/thirdPartyId`. Anders kunnen wijzigingen in het profiel inconsistent en onvoorspelbaar zijn.</li><li>Een nieuwe sessie-id moet worden gebruikt na 30 minuten inactiviteit van een bezoeker.</li><li>Dezelfde sessie-id gebruiken met meerdere `tntIds/thirdPartyIds` kan leiden tot onvoorspelbare wijzigingen in de profielen die worden geïdentificeerd door de `tntId/thirdPartyIDs`.</li></ul>OPMERKING: Zie [beperking van het aantal gelijktijdige aanvragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html#content-delivery){target=_blank} voor een bepaalde sessie-id.<P>**pc-id**: Een halfpermanente id voor de browser van een bezoeker. Hiermee wordt de duur van het programma verlengd totdat cookies handmatig worden verwijderd.<P>**controleren**: Een eenvoudige testwaarde die wordt gebruikt om te bepalen of een bezoeker cookies ondersteunt. Stel de instellingen in wanneer een bezoeker een pagina aanvraagt.<P>**disable**: Instellen als de laadtijd van een bezoeker de time-out overschrijdt die in het bestand at.js is geconfigureerd. Deze time-out duurt standaard één uur. |
| `at_check` | Tijdelijke cookie om te controleren of de functie voor lezen/schrijven van cookies is ingeschakeld in de browser. |
| `mboxEdgeCluster` | Deze cookies zijn alleen aanwezig wanneer/if [overrideMboxEdgeServer-instelling](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} is ingesteld op `true`. |

Het is niet mogelijk `HTTPOnly` op deze cookies van de eerste partij. De `at.js` JavaScript-bibliotheek moet naar deze cookies lezen/schrijven. Deze cookies worden gemaakt door `at.js` en zijn niet ingesteld vanaf de server.

De `secure` deze instelling kan voor al deze cookies worden ingeschakeld met de `secureOnly: true` configuratie in `at.js`.

## Cookies van andere bedrijven

Adobe Target-gebruikers kunnen aangepaste cookies van derden maken. De volgende cookies van andere leveranciers worden opgeslagen op `tt.omtrdc.net`:

| Cookie | Details |
| --- | --- |
| `customerclientcode!mboxPC` | Presenteren als cross-domain is ingeschakeld. |
| `customerclientcode!mboxSession` | Presenteren als cross-domain is ingeschakeld. |

Deze cookies van derden zijn HTTPOnly out of the box en worden ingesteld door Adobe Target-servers voor gegevensverzameling.

De `secure` deze instelling kan voor alle cookies worden ingeschakeld met de `secureOnly: true` configuratie in `at.js`.
