---
description: Leer hoe Adobe Target cookies gebruikt om websitebeheerders de mogelijkheid te bieden te testen welke online inhoud en aanbiedingen voor bezoekers relevanter zijn.
solution: Experience Cloud,Analytics,Target
title: Adobe Target cookies
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: a1d24f95b1ac567686d58af8adf0132e5beb8f2a
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Adobe Target cookies

[!DNL Adobe Target] gebruikt cookies om websitebeheerders in staat te stellen te testen welke online-inhoud en -aanbiedingen voor bezoekers relevanter zijn.

>[!NOTE]
>
>De informatie in dit artikel is van toepassing op [[!DNL Target] at.js JavaScript-bibliotheek](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} alleen.
>
>Voor informatie over cookies die worden gebruikt in een [!DNL Target] implementatie met behulp van de [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>U kunt de instellingen die in dit artikel worden besproken desgewenst wijzigen, behalve voor de duur van de cookie. [Vraag uw accountvertegenwoordiger](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} bij het wijzigen van cookie-instellingen.
>
>[!DNL Target] gebruikers kunnen ook aangepaste cookies van derden maken.

## Cookies van eerste bedrijven

De volgende cookies van de eerste fabrikant worden in het domein van de klant opgeslagen:

| Cookie | Details |
| --- | --- |
| mbox | Hiermee worden anonieme id&#39;s over de bezoeker opgeslagen.<P>**Cookie-domein**: Het domein waarvan u de mbox dient. Omdat deze cookie wordt aangeleverd vanaf het domein van uw bedrijf, is de cookie een cookie van de eerste partij. Voorbeeld: `mycompany.com`. Als een van uw domeinnamen een landcode bevat, zoals `mycompany.co.uk`, werk met uw Diensten van de Cliënt om at.js te vormen om deze code te steunen. Voor informatie over het aanpassen van het cookiedomein, indien nodig, zie &quot;`cookieDomain`&quot; onder [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} in de *[!DNL Adobe Target]Handleiding voor ontwikkelaars*.<P>**Serverdomein**: `clientcode.tt.omtrdc.net`, met de clientcode voor uw [!DNL Target] account.<P>**Duur van cookie**: Het cookie blijft twee jaar na de laatste aanmelding in de browser van de bezoeker staan. U kunt de duur van het cookie niet wijzigen.<P>Het cookie houdt enkele waarden bij om te beheren hoe uw bezoekers ervoeren [!DNL Target] activiteiten:<P>**sessie-id**: Een unieke id voor een bepaalde gebruikerssessie. Standaard verloopt de sessie na 30 minuten inactiviteit. Als u genereert `sessionId` uzelf (bijvoorbeeld [server-side implementaties](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), zorgt u voor het volgende:<ul><li>De sessie-id kan elke afdrukbare tekenreeks zijn, behalve een spatie, vraagteken ( ? ) of een schuine streep ( / ).</li><li>De sessie-id moet 1 tot 128 tekens lang zijn.</li><li>Voor een bepaalde sessie moet de waarde van het cookie gelijk blijven voor meerdere aanvragen.</li><li>U moet nooit parallelle sessies hebben (verschillend `sessionIds`) voor een bepaalde bezoeker op een bepaald tijdstip.</li></ul>Het verpletteren aan een bepaalde knoop in de randcluster wordt gedaan gebruikend zitting-identiteitskaart.<ul><li>De sessie is 30 minuten actief aan de serverzijde. Daarom zou u geen verschillende zitting-identiteitskaart voor een bepaald moeten gebruiken `tntId/thirdPartyId` binnen 30 minuten na het laatste verzoek bij het `tntId/thirdPartyId`. Anders kunnen wijzigingen in het profiel inconsistent en onvoorspelbaar zijn.</li><li>Een nieuwe sessie-id moet worden gebruikt na 30 minuten inactiviteit van een bezoeker.</li><li>Dezelfde sessie-id gebruiken met meerdere `tntIds/thirdPartyIds` kan leiden tot onvoorspelbare wijzigingen in de profielen die door de `tntId/thirdPartyIDs`.</li></ul>OPMERKING: Zie [beperking van het aantal gelijktijdige aanvragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=en#content-delivery){target=_blank} voor een bepaalde sessie-id.<P>**pc-id**: Een halfpermanente id voor de browser van een bezoeker. Hiermee wordt de duur van de cookies gewijzigd totdat de cookies handmatig worden verwijderd.<P>**controleren**: Een eenvoudige testwaarde die wordt gebruikt om te bepalen of een bezoeker cookies ondersteunt. Stel de instellingen in wanneer een bezoeker een pagina aanvraagt.<P>**disable**: Stel in of de laadtijd van een bezoeker langer is dan de time-out die is geconfigureerd in het bestand at.js. Deze time-out duurt standaard één uur. |
| at_check | Tijdelijke cookie om te controleren of de functie voor lezen/schrijven van cookies is ingeschakeld in de browser. |
| mboxEdgeCluster | Deze cookies zijn alleen aanwezig wanneer/if [overrideMboxEdgeServer-instelling](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} is ingesteld op `true`. |

Het is niet mogelijk om HTTPO alleen op deze eerstehulpkoekjes te gebruiken. De JavaScript-bibliotheek at.js moet naar deze cookies lezen/schrijven. Deze cookies worden gemaakt door at.js en worden niet ingesteld vanaf de server.

De `secure` deze instelling kan voor al deze cookies worden ingeschakeld met de `secureOnly: true` configuratie in de at.js implementatie.

## Cookies van andere bedrijven

De volgende cookies van andere leveranciers worden opgeslagen op `tt.omtrdc.net`:

| Cookie | Details |
| --- | --- |
| customerclientcode!mboxPC | Deze cookie is aanwezig als cross-domain is ingeschakeld. |
| customerclientcode!mboxSession | Deze cookie is aanwezig als cross-domain is ingeschakeld. |

Deze cookies van andere leveranciers zijn HTTPOnly out of the box en worden ingesteld door de [!DNL Target] Edge-servers.

De `secure` deze instelling kan voor alle cookies worden ingeschakeld met de `secureOnly: true` configuratie in de at.js implementatie.