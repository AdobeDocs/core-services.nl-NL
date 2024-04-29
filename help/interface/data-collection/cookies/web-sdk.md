---
title: Adobe Experience Platform Web SDK cookies
description: Leer hoe de SDK van het Web koekjes gebruikt die op uw implementatie van toepassing zijn.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
source-git-commit: 66f78a04674a82335f5df20c4c15d983b6ebdc66
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Adobe Experience Platform Web SDK cookies

De Adobe Experience Platform Web SDK gebruikt cookies om waarden op te slaan die specifiek zijn voor uw implementatie.

| Naam | Max. leeftijd | Beschrijving |
|---|---|---|
| **kndct_orgid_identity** | 34128000 (395 dagen) | Hiermee slaat u de ECID op, evenals andere informatie over de ECID. |
| **kndctr_orgid_permission_check** | 7200 (2 uur) | Hiermee geeft u aan dat de server de voorkeursserver voor toestemming moet opzoeken. |
| **kndctr_orgid_permission** | 15552000 (180 dagen) | Hiermee slaat u de voorkeur van de gebruiker voor toestemming voor de website op. |
| **kndctr_orgid_cluster** | 1800 (30 minuten) | Hiermee slaat u het gebied Edge Network op dat de verzoeken van de huidige gebruiker dient. Het gebied wordt gebruikt in de weg URL zodat de Edge Network het verzoek aan het correcte gebied kan leiden. Als een gebruiker met een verschillend IP adres of in een verschillende zitting verbindt, wordt het verzoek opnieuw verpletterd aan het dichtstbijzijnde gebied. |
| **mbox** | 63072000 | Aanwezig wanneer het Doel migratie plaatsen aan waar is. Het laat het Doel toe [mbox cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) in te stellen door de Web SDK. |
| **mboxEdgeCluster** | 1800 (30 minuten) | Aanwezig wanneer het Doel migratie plaatsen aan waar is. Het staat SDK van het Web toe om de correcte randcluster aan mee te delen `at.js` zodat doelprofielen synchroon blijven wanneer gebruikers door een site navigeren. |
| **AMCV_##@AdobeOrg** | 34128000 (395 dagen) | Presenteren wanneer [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) is ingeschakeld. Het helpt wanneer het overgaan naar Web SDK terwijl sommige delen van de plaats nog gebruiken `visitor.js`. |

De Edge Network stelt alle cookies in met de `secure` en `sameSite="none"` kenmerken. Als u momenteel zowel beveiligde als niet-beveiligde secties op uw website hebt, is de gebruikersidentificatie mogelijk onjuist. Wanneer een gebruiker van een veilige sectie van de plaats aan een onveilige sectie navigeert, produceert de Edge Network een nieuw `ECID` met het verzoek.
