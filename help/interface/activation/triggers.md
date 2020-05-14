---
description: Hoe u Experience Cloud Triggers configureert.
keywords: integrations;Triggers
seo-description: Hoe u Experience Cloud Triggers configureert.
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: fb03bf89bcc6ed4438daf18c8415de3052ba8fa4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---


# Triggers

## Overzicht van triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

Met triggers kunt u belangrijke vormen van consumentengedrag identificeren, definiëren en controleren en vervolgens communicatie tussen oplossingen genereren om bezoekers opnieuw aan te trekken. U kunt triggers gebruiken in realtime beslissingen en personalisatie.

* Snel opnieuw op de markt brengen voor winkels met winkelwagentjes of winkels met winkels met winkels met winkels en winkels met verwijderde producten configureren
* Incomplete formulieren en toepassingen
* Handelingen of reeksen handelingen op de site

![](assets/trigger-abandonment-2.png)

### Typen triggers

Over het algemeen kan het 15 tot 90 minuten duren voordat een marketingcampagne wordt gestart. Dit hangt van de implementatie van gegevensinzameling, lading op de pijpleiding, douaneconfiguratie van de bepaalde trekker, en het werkschema in de Campagne van Adobe af.

* **Afschaffing:** U kunt een trigger maken die moet worden geactiveerd wanneer een bezoeker een product weergeeft, maar er niets aan toevoegt.
* **Handeling:** U kunt bijvoorbeeld triggers maken om na aanmelding voor nieuwsbrieven, e-mailabonnementen of aanvragen voor creditcards (bevestigingen) te activeren. Als u een detailhandelaar bent, kunt u een trekker voor een bezoeker tot stand brengen die zich voor een loyaliteitsprogramma ondertekent. In media en vermaak, creeer trekkers voor bezoekers die op een bepaalde show letten, en misschien wilt u met een onderzoek antwoorden.
* **Begin en einde sessie:** Maak een trigger voor het starten en beëindigen van de sessie.

## Een Experience Cloud-trigger maken {#task_821F37183AC045E5AC8EED20317598FE}

Maak een trigger en configureer de voorwaarden voor de trigger. U kunt bijvoorbeeld de criteria voor de regels van een trigger tijdens een bezoek opgeven, zoals maateenheden zoals Kart Abandon of afmetingen zoals de productnaam. Wanneer aan de regels wordt voldaan, loopt de trekker.

>[!NOTE]
>
>Er bestaat momenteel een technische limiet van 100 triggers.

1. Klik in de Experience Cloud op ![](assets/menu-icon.png)en klik op **[!UICONTROL Launch]**.
2. Zoek de [!UICONTROL Triggers] kaart en klik op **[!UICONTROL Manage Triggers]**.
3. Klik **[!UICONTROL New Trigger]** en geef vervolgens het type trigger op:

   ![Stap resultaat](assets/add-trigger.png)

4. Vorm de trekker door de volgende gebieden te voltooien en metriek en afmetingspunten aan de containers van de regel te slepen:

   | Element | Beschrijving |
   |--- |--- |
   | Naam | De vriendelijke naam voor deze trigger. |
   | Beschrijving | De beschrijving van deze trigger, hoe u deze gaat gebruiken enzovoort. |
   | Rapportsuite | De [rapportsuite](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html) Analytics die voor deze trigger wordt gebruikt. Deze instelling identificeert de te gebruiken rapportgegevens. |
   | Bezoek moet<br>includeVisit mag geen<br>includeTrigger zijn na geen<br>actionInclusief metagegevens | U kunt criteria of gedrag van bezoekers bepalen die u wilt voorkomen, en gedrag dat u niet wilt voorkomen.  De regels voor een eenvoudige activering van een winkelwagentje kunnen bijvoorbeeld als volgt zijn:<ul><li>Het bezoek moet het volgende omvatten:  Kart optellen (metrisch) en bestaat. (U kunt de regel verder verfijnen met een specifieke productweergave of met afmetingen zoals Browsertypen.)</li><li>Bezoek mag niet omvatten:  Afhandeling.</li><li>Trigger na geen actie voor:  10 minuten.</li><li>Inclusief metagegevens: Hiermee kunt u een bepaalde dimensie of variabelen toevoegen die relevant zijn voor het gedrag van een bezoeker. Dit veld kan handig zijn voor Adobe Campaign om de juiste e-mail voor opnieuw marketing te maken.</li></ul><br>U kunt om het even welk, en of logica binnen of tussen containers specificeren, afhankelijk van de criteria u belangrijk voor de regel bepaalt. |
   | Container | In containers kunt u regels, voorwaarden of filters instellen en opslaan die een trigger definiëren. Als u wilt dat gebeurtenissen tegelijkertijd plaatsvinden, plaatst u ze in dezelfde container. Met andere woorden, elke container verwerkt onafhankelijk op raakniveau.  Bijvoorbeeld, als u twee containers hebt die door de exploitant worden aangesloten van En, kunt u de regels verwachten om te kwalificeren wanneer twee klappen aan de vereisten voldoen. |
   | Nieuwe sessie starten na | Maak een trigger voor het starten en beëindigen van de sessie. |

5. Klik op **[!UICONTROL Save]**.
6. Gebruik triggers voor [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Voorbeeld triggers

Voorbeelden van Experience Cloud-triggers:

#### Trigger voor weglating van winkelwagentje

De volgende pagina bevat bijvoorbeeld regels die u kunt gebruiken voor een trigger voor het afbreken van winkelwagentjes, op basis van producten die tijdens een bezoek worden weergegeven.

![](assets/abandonment-trigger.png)

#### Referrer Trigger

De volgende trigger wordt geactiveerd wanneer een treffer wordt geleverd met het product van Men&#39;s Boots en referentie van Facebook. Om de twee criteria (*producten* en *referentie*) in dezelfde hit te kunnen beoordelen, moeten ze aan dezelfde container worden toegevoegd.

![](assets/fb-boots-promo.png)
