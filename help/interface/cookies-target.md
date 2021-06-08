---
description: Leer hoe Adobe Target cookies gebruikt om websitebeheerders de mogelijkheid te bieden te testen welke online inhoud en aanbiedingen voor bezoekers relevanter zijn.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target,Social
title: 'Adobe Target Cookies '
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Beheer
role: Administrator
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: c7ed1324015beb7ebcf7a4ee21b05601e36e608f
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 1%

---

# Adobe Target Cookies{#target-cookies}

Adobe Target gebruikt cookies om websitebeheerders de mogelijkheid te bieden te testen welke online-inhoud en aanbiedingen voor bezoekers relevanter zijn.

U kunt deze instellingen desgewenst wijzigen, behalve voor de duur van het cookie. Vraag uw accountvertegenwoordiger wanneer u de cookie-instellingen wijzigt.

>[!NOTE]
>
>Adobe Target-gebruikers kunnen ook aangepaste cookies van derden maken.

| Instelling | Informatie |
| --- | --- |
| Naam cookie | mbox. |
| Cookie-domein | De tweede en hoogste niveaus van de domeinen waarvan u de mbox dienen. Omdat het van het domein van uw bedrijf wordt gediend, is het koekje een eerste partijkoekje. Voorbeeld: `mycompany.com`. |
| Serverdomein | `clientcode.tt.omtrdc.net`, met de clientcode voor uw  [!DNL Adobe Target] account. |
| Duur van cookie | Het cookie blijft twee jaar na de laatste aanmelding in de browser van de bezoeker staan. U kunt de duur van het cookie niet wijzigen. |

>[!NOTE]
>
>Als om het even welk van uw domeinnamen een landcode, zoals `mycompany.co.uk` omvatten, werk met uw Diensten van de Cliënt om uw `at.js` te vormen om deze code te steunen.

Het cookie houdt enkele waarden bij voor het beheren van de manier waarop bezoekers campagnes van Adobe Target ervaren:

| Waarde | Definitie |
| --- | --- |
| sessie-id | Een unieke id voor een bepaalde gebruikerssessie. Standaard verloopt de sessie na 30 minuten inactiviteit. Als u sessionId zelf (bijvoorbeeld, voor server-zijimplementaties) produceert, zorg het volgende ervoor:<ul><li>De sessie-id kan elke afdrukbare tekenreeks zijn, behalve een spatie, vraagteken ( ? ) of een schuine streep ( / ).</li><li>* De sessie-id moet 1 tot 128 tekens lang zijn.</li><li>Voor een bepaalde zitting moet zijn waarde het zelfde over veelvoudige verzoeken blijven</li><li>U zou nooit parallelle zittingen (verschillende sessionIds) voor een bepaalde bezoeker op om het even welk ogenblik moeten hebben.</li></ul>Het verpletteren aan een bepaalde knoop in de randcluster wordt gedaan gebruikend identiteitskaart van de Zitting.<ul><li>De sessie is 30 minuten actief aan de serverzijde. Daarom moet u geen verschillende Zitting ID voor een bepaalde `tntId/thirdPartyId` binnen 30 minuten van het laatste verzoek gebruiken die met `tntId/thirdPartyId` wordt gemaakt. Anders kunnen wijzigingen in het profiel inconsistent en onvoorspelbaar zijn.</li><li>Als u dezelfde sessie-id gebruikt met meerdere `tntIds/thirdPartyIds`, kunnen er onvoorspelbare wijzigingen optreden in de profielen die worden aangeduid door `tntId/thirdPartyIDs`.</li></ul> |
| pc-id | Een halfpermanente id voor de browser van een bezoeker. Hiermee wordt de duur van de cookies gewijzigd totdat de cookies handmatig worden verwijderd. |
| controleren | Een eenvoudige testwaarde die wordt gebruikt om te bepalen of een bezoeker cookies ondersteunt. Stel de instellingen in wanneer een bezoeker een pagina aanvraagt. |
| disable | Stel in of de laadtijd van de bezoeker langer is dan de time-out die is geconfigureerd in het bestand at.js. Deze time-out duurt standaard 1 uur. |

