---
title: Adobe Experience Platform Web SDK Cookies
description: Leer hoe de SDK van het Web koekjes gebruikt die op uw implementatie van toepassing zijn.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
source-git-commit: d69af76f6deff4f2b73e67ee7b69b9fee1ee3a2e
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Adobe Experience Platform Web SDK cookies

De Adobe Experience Platform Web SDK gebruikt cookies om waarden op te slaan die specifiek zijn voor uw implementatie.

| Naam | Max. leeftijd | Grootte | Beschrijving |
|---|---|---|---|
| **kndctr_&lt;ORG_ID>_identity** | 34128000 (395 dagen) | 100-120 bytes (variabele) | Hiermee slaat u de ECID op, evenals andere informatie over de ECID. |
| **kndctr_&lt;ORG_ID>_permission** | 15552000 (180 dagen) | 10-11 bytes | Hiermee slaat u de voorkeur van de gebruiker voor toestemming voor de website op. |
| **kndctr_&lt;ORG_ID>_cluster** | 1800 (30 minuten) | 3-5 bytes | Hiermee slaat u het gebied Edge Network op dat de verzoeken van de huidige gebruiker dient. Het gebied wordt gebruikt in de weg URL zodat de Edge Network het verzoek aan het correcte gebied kan leiden. Als een gebruiker met een verschillend IP adres of in een verschillende zitting verbindt, wordt het verzoek opnieuw verpletterd aan het dichtstbijzijnde gebied. |
| **mbox** | 63072000 | | Aanwezig wanneer het Doel migratie plaatsen aan waar is. Het staat het 3&rbrace; mbox koekje van het Doel [&#128279;](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) toe om door het Web SDK worden geplaatst. |
| **mboxEdgeCluster** | 1800 (30 minuten) | | Aanwezig wanneer het Doel migratie plaatsen aan waar is. Hiermee kan de SDK van het Web de juiste Edge-cluster aan `at.js` meedelen, zodat de doelprofielen synchroon kunnen blijven terwijl gebruikers door een site navigeren. |
| **AMCV_##@AdobeOrg** | 34128000 (395 dagen) | | Presenteren wanneer [`idMigrationEnabled` ](https://experienceleague.adobe.com/nl/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) wordt toegelaten. Het helpt bij het overschakelen naar Web SDK terwijl sommige delen van de site nog steeds `visitor.js` gebruiken. |

De Edge Network stelt alle cookies in met de kenmerken `secure` en `sameSite="none"` . Als u momenteel zowel beveiligde als niet-beveiligde secties op uw website hebt, is de gebruikersidentificatie mogelijk onjuist. Wanneer een gebruiker van een beveiligde sectie van de site naar een niet-beveiligde sectie navigeert, genereert de Edge Network een nieuwe `ECID` met de aanvraag.
