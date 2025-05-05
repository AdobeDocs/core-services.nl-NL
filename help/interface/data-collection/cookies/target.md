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
>De informatie in dit artikel is slechts op de [ bibliotheek van JavaScript van Adobe Target ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=nl-NL){target=_blank} van toepassing  (`at.js`). Zie [ de koekjes van SDK van het Web van Adobe Experience Platform ](web-sdk.md) voor informatie over de implementaties van het Doel gebruikend SDK van het Web.
>
>U kunt de instellingen die in dit artikel worden besproken, indien nodig wijzigen, behalve voor de duur van de cookie. [ raadpleeg uw rekeningsvertegenwoordiger ](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html?lang=nl-NL){target=_blank}  wanneer het veranderen van koekjesmontages.

## Cookies van eerste bedrijven

De volgende cookies van de eerste fabrikant worden in het domein van de klant opgeslagen:

| Cookie | Details |
| --- | --- |
| `mbox` | Hiermee worden anonieme id&#39;s over de bezoeker opgeslagen.<P>**domein van het Koekje**: Het domein waarvan u mbox dient. Omdat deze cookie wordt aangeleverd vanaf het domein van uw bedrijf, is de cookie een cookie van de eerste partij. Als een van uw domeinnamen een landcode bevat, zoals `example.co.uk` , werkt u samen met Client Services om `at.js` zo te configureren dat deze code wordt ondersteund. Voor informatie over het aanpassen van het koekjesdomein, indien nodig, zie `cookieDomain` onder [ targetGlobalSettings ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=nl-NL){target=_blank}  in de de ontwikkelaarsgids van Adobe Target.<P>**het domein van de Server**: `clientcode.tt.omtrdc.net`, gebruikend de cliëntcode voor uw rekening van Adobe Target.<P>**duur van het Koekje**: Het koekje blijft op browser van de bezoeker twee jaar van laatste login. U kunt de duur van het cookie niet wijzigen.<P>De cookie houdt enkele waarden bij om te beheren hoe uw bezoekers [!DNL Target] -activiteiten ervaren:<P>**zitting identiteitskaart**: Een uniek herkenningsteken voor een bepaalde gebruikerszitting. Standaard verloopt de sessie na 30 minuten inactiviteit. Als u `sessionId` zelf (bijvoorbeeld, voor [ server-zijimplementaties ](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html?lang=nl-NL){target=_blank} ) produceert, verzeker het volgende:<ul><li>De sessie-id kan elke afdrukbare tekenreeks zijn, behalve een spatie, vraagteken ( ? ) of een schuine streep ( / ).</li><li>De sessie-id moet 1 tot 128 tekens lang zijn.</li><li>Voor een bepaalde sessie moet de waarde van het cookie gelijk blijven voor meerdere aanvragen.</li><li>U mag nooit parallelle sessies (verschillend `sessionIds`) voor een bepaalde bezoeker hebben op een bepaald moment.</li></ul>Het verpletteren aan een bepaalde knoop in de randcluster wordt gedaan gebruikend zitting-identiteitskaart.<ul><li>De sessie is 30 minuten actief op de server. Daarom moet u geen andere sessie-id gebruiken voor een bepaalde `tntId/thirdPartyId` binnen 30 minuten na de laatste aanvraag die u met de `tntId/thirdPartyId` hebt gedaan. Anders kunnen wijzigingen in het profiel inconsistent en onvoorspelbaar zijn.</li><li>Een nieuwe sessie-id moet worden gebruikt na 30 minuten inactiviteit van een bezoeker.</li><li>Als dezelfde sessie-id met meerdere `tntIds/thirdPartyIds` wordt gebruikt, kunnen er onvoorspelbare wijzigingen optreden in de profielen die door `tntId/thirdPartyIDs` worden geïdentificeerd.</li></ul>NOTA: Zie [ grens op aantal gezamenlijke verzoeken ](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=nl-NL#content-delivery){target=_blank}  voor een bepaalde zittingsidentiteitskaart<P>**pc identiteitskaart**: Een semi-permanente identiteitskaart voor browser van een bezoeker. Hiermee wordt de duur van het programma verlengd totdat cookies handmatig worden verwijderd.<P>**controle**: Een eenvoudige testwaarde die wordt gebruikt om te bepalen als een bezoeker koekjes steunt. Stel de instellingen in wanneer een bezoeker een pagina aanvraagt.<P>**maak** onbruikbaar: Plaats als de ladingstijd van een bezoeker de onderbreking overschrijdt die in het at.js- dossier wordt gevormd. Deze time-out duurt standaard één uur. |
| `at_check` | Tijdelijke cookie om te controleren of de functie voor lezen/schrijven van cookies is ingeschakeld in de browser. |
| `mboxEdgeCluster` | Deze koekjes zijn slechts aanwezig wanneer/als [ overrideMboxEdgeServer plaatsend ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=nl-NL){target=_blank}  aan `true` wordt geplaatst. |

Het is niet mogelijk `HTTPOnly` te gebruiken voor deze cookies van de eerste fabrikant. De `at.js` JavaScript-bibliotheek moet naar deze cookies lezen/schrijven. Deze cookies worden gemaakt door `at.js` en worden niet ingesteld vanaf de server.

De instelling `secure` kan voor al deze cookies worden ingeschakeld met de configuratie `secureOnly: true` in `at.js` .

## Cookies van andere bedrijven

Adobe Target-gebruikers kunnen aangepaste cookies van derden maken. De volgende cookies van derden worden opgeslagen op `tt.omtrdc.net` :

| Cookie | Details |
| --- | --- |
| `customerclientcode!mboxPC` | Presenteren als cross-domain is ingeschakeld. |
| `customerclientcode!mboxSession` | Presenteren als cross-domain is ingeschakeld. |

Deze cookies van derden zijn HTTPOnly out of the box en worden ingesteld door Adobe Target-servers voor gegevensverzameling.

De instelling `secure` kan voor alle cookies worden ingeschakeld met de configuratie `secureOnly: true` in `at.js` .
