---
title: Regionale gegevensverzameling
description: Informatie over regionale gegevensverzameling
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
source-git-commit: 01851c4d66cbaf1a68961b86926e8cc2c310d1ec
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Regionale gegevensverzameling

De Adobe Experience Cloud maakt gebruik van regionale gegevensverzameling (RDC), zodat interacties tussen uw bezoekers en Adobe zo dicht mogelijk bij uw bezoekers plaatsvinden. Gegevens die lokaal op een randsite zijn verzameld, worden veilig doorgestuurd naar een kernsite voor verwerking. Na verwerking zijn de gegevens beschikbaar voor Adobe Experience Cloud-producten en -services.

De workflow voor regionale gegevensverzameling biedt verschillende voordelen:

* **Prestaties**: Met RDC, verbinden uw bezoekers met de dichtste randplaats. Deze optimalisatie biedt de snelste responstijd, wat resulteert in nauwkeurigere tracking en snellere laadtijden.
* **Overtolligheid**: Als er een verstoring in communicatie tussen om het even welke plaats van de randplaats en kernplaats is, bewaart de infrastructuur van de Adobe plaatselijk gegevens, dan door:sturen het aan de kernplaats wanneer de mededelingen worden hersteld. De Adobe kan verkeer aan andere randplaatsen ook leiden als een specifieke plaats onderbrekingen ervaart.

De regionale distributiesector omvat momenteel de volgende locaties (afhankelijk van de verandering):

## Gegevensverzameling van eerste partijen

| RDC-type | Centra voor gegevensverzameling |
| --- | --- |
| Algemeen (standaard) | Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |
| Wereldwijd + China* | Beijing*, Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |
| Alleen Amerika | Oregon, Virginia |
| Alleen Europa | Ierland, Parijs |
| Alleen Azië-Stille Oceaan | Mumbai, Singapore, Tokio, Sydney |
| Alleen China* | Peking |

{style="table-layout:auto"}

_*China RDC vereist het China Performance Optimization add-on pakket en is alleen van toepassing op Adobe Analytics dat gebruik maakt van het verzamelen van gegevens van AppMeasurementen. De andere diensten van het Experience Cloud en de gegevensinzameling van SDK van het Web worden niet gesteund. Neem contact op met het accountteam van de Adobe voor meer informatie over het add-onpakket voor de optimalisatie van de prestaties van China._

## Gegevensverzameling van derden

Gegevensverzameling van derden omvat cookiedomeinen die niet overeenkomen met uw websitedomein. Voorbeelden zijn `adobedc.net` , `omtrdc.net` en `2o7.net` .

| RDC-type | Centra voor gegevensverzameling |
| --- | --- |
| Standaard | Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |
| Standaard + China* | Beijing*, Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |

{style="table-layout:auto"}
