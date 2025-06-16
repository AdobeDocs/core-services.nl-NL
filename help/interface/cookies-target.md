---
description: Leer hoe  [!DNL Adobe Target]  koekjes gebruikt om websiteexploitanten de capaciteit te geven om te testen welke online inhoud en aanbiedingen voor bezoekers relevanter zijn.
solution: Experience Cloud,Analytics,Target
title: Adobe Target cookies
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 3ca021a0a2e6b0b6e265d35084d89d7720c28908
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Adobe Target cookies

[!DNL Adobe Target] gebruikt cookies om websitebeheerders de mogelijkheid te bieden te testen welke online-inhoud en -aanbiedingen voor bezoekers relevanter zijn.

>[!NOTE]
>
>De informatie in dit artikel is op [[!DNL Target]  at.js slechts de bibliotheek van JavaScript ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} van toepassing.
>
>Voor informatie over koekjes die in een [!DNL Target] implementatie gebruikend [[!DNL Adobe Experience Platform Web SDK] worden gebruikt ](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html){target=_blank}, zie &quot;gebruiken de [!DNL Adobe Experience Platform Web SDK] koekjes? Zo ja, welke cookies gebruikt zij?&quot; in [[!DNL Veelgestelde vragen in de het overzichtsgids van SDK van het Platform van &#x200B;]](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>U kunt de instellingen die in dit artikel worden besproken, indien nodig wijzigen, behalve voor de duur van de cookie. [ raadpleeg uw accountvertegenwoordiger ](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} wanneer het veranderen van koekjesmontages.
>
>[!DNL Target] -gebruikers kunnen ook aangepaste cookies van derden maken.

## Cookies van eerste bedrijven

De volgende cookies van de eerste fabrikant worden in het domein van de klant opgeslagen:

| Cookie | Details |
| --- | --- |
| mbox | Hiermee worden anonieme id&#39;s over de bezoeker opgeslagen.<P>**domein van het Koekje**: Het domein waarvan u mbox dient. Omdat deze cookie wordt aangeleverd vanaf het domein van uw bedrijf, is de cookie een cookie van de eerste partij. Voorbeeld: `mycompany.com` . Als om het even welk van uw domeinnamen een landcode, zoals `mycompany.co.uk` omvatten, werk met uw Diensten van de Cliënt om at.js te vormen om deze code te steunen. Voor informatie over het aanpassen van het koekjesdomein, indien nodig, zie &quot;`cookieDomain`&quot; onder [ targetGlobalSettings ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} in de *[!DNL Adobe Target]Gids van de Ontwikkelaar*.<P>**het domein van de Server**: `clientcode.tt.omtrdc.net`, gebruikend de cliëntcode voor uw [!DNL Target] rekening.<P>**duur van het Koekje**: Het koekje blijft op browser van de bezoeker twee jaar van laatste login. U kunt de duur van het cookie niet wijzigen.<P>De cookie houdt enkele waarden bij om te beheren hoe uw bezoekers [!DNL Target] -activiteiten ervaren:<P>**zitting identiteitskaart**: Een uniek herkenningsteken voor een bepaalde gebruikerszitting. Standaard verloopt de sessie na 30 minuten inactiviteit. Als u `sessionId` zelf (bijvoorbeeld, voor [ server-zijimplementaties ](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}) produceert, zorg het volgende ervoor:<ul><li>De sessie-id kan elke afdrukbare tekenreeks zijn, behalve een spatie, vraagteken ( ? ), accolades ( { } ) of een schuine streep ( / ).</li><li>De sessie-id moet 1 tot 128 tekens lang zijn.</li><li>Voor een bepaalde sessie moet de waarde van het cookie gelijk blijven voor meerdere aanvragen.</li><li>U mag nooit parallelle sessies (verschillend `sessionIds`) voor een bepaalde bezoeker hebben op een bepaald moment.</li></ul>Het verpletteren aan een bepaalde knoop in de randcluster wordt gedaan gebruikend zitting-identiteitskaart.<ul><li>De sessie is 30 minuten actief op de server. Daarom moet u geen andere sessie-id gebruiken voor een bepaalde `tntId/thirdPartyId` binnen 30 minuten na de laatste aanvraag die u met de `tntId/thirdPartyId` hebt gedaan. Anders kunnen wijzigingen in het profiel inconsistent en onvoorspelbaar zijn.</li><li>Een nieuwe sessie-id moet worden gebruikt na 30 minuten inactiviteit van een bezoeker.</li><li>Als dezelfde sessie-id met meerdere `tntIds/thirdPartyIds` wordt gebruikt, kunnen er onvoorspelbare wijzigingen optreden in de profielen die door `tntId/thirdPartyIDs` worden geïdentificeerd.</li></ul>NOTA: Zie [ grens op aantal gezamenlijke verzoeken ](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=en#content-delivery){target=_blank} voor een bepaalde zittingsidentiteitskaart<P>**pc identiteitskaart**: Een semi-permanente identiteitskaart voor browser van een bezoeker. Hiermee wordt de duur van het programma verlengd totdat cookies handmatig worden verwijderd.<P>**controle**: Een eenvoudige testwaarde die wordt gebruikt om te bepalen als een bezoeker koekjes steunt. Stel de instellingen in wanneer een bezoeker een pagina aanvraagt.<P>**maak** onbruikbaar: Plaats als de ladingstijd van een bezoeker de onderbreking overschrijdt die in het at.js- dossier wordt gevormd. Deze time-out duurt standaard één uur. |
| at_check | Tijdelijke cookie om te controleren of de functie voor lezen/schrijven van cookies is ingeschakeld in de browser. |
| mboxEdgeCluster | Deze koekjes zijn slechts aanwezig wanneer/als [ overrideMboxEdgeServer plaatsend ](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} aan `true` wordt geplaatst. |

Het is niet mogelijk om HTTPO alleen op deze eerstehulpkoekjes te gebruiken. De JavaScript-bibliotheek at.js moet deze cookies lezen/schrijven. Deze cookies worden gemaakt door at.js en worden niet ingesteld vanaf de server.

De instelling `secure` kan voor al deze cookies worden ingeschakeld met de configuratie `secureOnly: true` in de implementatie at.js.

## Cookies van andere bedrijven

De volgende cookies van derden worden opgeslagen op `tt.omtrdc.net` :

| Cookie | Details |
| --- | --- |
| customerclientcode!mboxPC | Deze cookie is aanwezig als cross-domain is ingeschakeld. |
| customerclientcode!mboxSession | Deze cookie is aanwezig als cross-domain is ingeschakeld. |

Deze cookies van andere leveranciers zijn HTTPOnly out of the box en worden ingesteld door de Edge-servers van [!DNL Target] .

De instelling `secure` kan voor alle cookies worden ingeschakeld met de configuratie `secureOnly: true` in de implementatie at.js.