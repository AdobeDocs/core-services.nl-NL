---
description: Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.
seo-description: Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.
seo-title: Kaart rapportsuites aan een organisatie
title: Kaart rapportsuites aan een organisatie
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: af0bb1497252afa9bca2d6c7bacb11749cfe654c
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 1%

---


# Kaart rapportsuites aan een organisatie {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.

<!-- May 5 2020: This feature will likely be deprecated in Nov 2020. Any users with outstanding report suites that are not mapped will have 6 months to map their RS. -->

Experience Cloud-services (zoals Experience Cloud ID Service en [!UICONTROL People]) zijn gekoppeld aan een organisatie in plaats van aan een afzonderlijke rapportsuite. Om ervoor te zorgen dat deze services correct werken, moet elke Analytics-rapportensuite aan een organisatie worden toegewezen. Het toewijzingsproces:

* Plaatst een organisatie van Experience Cloud als primaire organisatie voor de rapportreeks.
* Hiermee wijzigt u niet wie toegang heeft tot een rapportsuite (de toegang wordt nog steeds bepaald door de Adobe Analytics-aanmeldingsaccount voor elke gebruiker)

## Vereisten

U moet een beheerder van Analytics van een login bedrijf zijn dat toegang tot de rapportreeks heeft u wilt in kaart brengen. Bovendien moet deze rekening aan een organisatie [van Experience Cloud worden](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) verbonden om rapportreeksen aan die organisatie in kaart te brengen.

Organisaties worden grijs weergegeven als u geen Analytics-beheerdersmachtigingen hebt voor een aanmeldingsbedrijf onder die organisatie die toegang heeft tot de opgegeven rapportsuite.

## Een rapportsuite toewijzen aan een organisatie {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Navigeer naar Rapporten Suites voor Data Governance op [!DNL Analytics] > **[!UICONTROL Admin]** > **[!UICONTROL Data Governance]** (zie de Plaatsing van het Beheer van Gegevens van het Suite van het Rapport [bekijken/beheren)](https://docs.adobe.com/help/en/analytics/admin/data-governance/gdpr-view-settings.html)

1. Om de login bedrijven te zien die toegang tot elke rapportreeks hebben, klik **[!UICONTROL Visible to Login Companies]**.

   Deze mening is bedoeld om u te helpen een geïnformeerde beslissing over de afbeelding nemen.

1. Klik drop-down in de **[!UICONTROL Mapped Organization]** kolom naast een rapportreeks en selecteer de organisatie waaraan u wilt in kaart brengen.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

## Meerdere rapportsuites toewijzen aan een organisatie {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Klik op **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**.

1. Selecteer de rapportsuites die u wilt in kaart brengen.

   ![](assets/rs-mapping-multiple.png)

1. Selecteer de organisatie (Outdoor Inc, in dit voorbeeld), dan klik **[!UICONTROL Select]**.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

1. Klik op **[!UICONTROL Save Mapping]**.

## Tips voor het selecteren van een Experience Cloud-organisatie {#mapping-tips}

Deze sectie bevat tips waarmee u de Experience Cloud-organisatie kunt selecteren waaraan u een rapportsuite moet toewijzen.

### Welke organisatie moet ik kiezen?

Als de Experience Cloud-id-service momenteel wordt geïmplementeerd in de rapportsuite, moet u ervoor zorgen dat de organisatie die u selecteert in het hulpprogramma voor het toewijzen van de rapportsuite dezelfde organisatie is als die is opgegeven in het [!DNL visitorAPI.js] bestand op uw site. U kunt de instructies in de [Test gebruiken en de Dienst](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) van identiteitskaart van Experience Cloud verifiëren om org identiteitskaart te vinden die door de dienst van identiteitskaart van de Bezoeker wordt gebruikt.

Als de dienst van identiteitskaart van de Bezoeker nog niet op de plaatsen wordt opgesteld die gegevens voor de rapportreeks verzamelen, als u de dienst van identiteitskaart van de Bezoeker van Experience Cloud in de toekomst opstelt, zult u moeten verzekeren uw plaatsing de organisatie aanpast u in het hulpmiddel van de Afbeelding van de Reeks van het Rapport koos.

### Waarom worden sommige organisaties gegraveerd?

Dit wijst erop dat u niet genoeg voorrechten hebt om aan de grayed-uit rapportreeks in kaart te brengen. Bekijk het volgende voorbeeld:

![](assets/rs-mapping.png)

In dit diagram geeft de blauwe sleutel beheerdersrechten aan. De grijze lijnen geven de zichtbaarheid aan.

Deze gebruiker heeft toegang tot twee Experience Cloud-organisaties. Hij heeft het volgende gedaan:

* Koppelde zijn beheerdersaccount in het [!UICONTROL chapek] Analytics-aanmeldingsbedrijf aan zijn [!UICONTROL Chapek] Corp Experience Cloud-organisatieaccount.
* Koppelde zijn niet-beheerdersaccount in het [!UICONTROL doohan] Analytics-aanmeldingsbedrijf aan zijn [!UICONTROL Chapek] Corp Experience Cloud-organisatieaccount.
* Koppelde zijn niet-beheerdersaccount in de nigel Analytics aanmeldmaatschappij aan zijn Nigel Inc Experience Cloud org account.

De volgende punten geven een overzicht van de toewijzingsacties die deze gebruiker kan en kan uitvoeren met betrekking tot deze rapportsuites:

* [!UICONTROL Chapek-prod] rapportsuite kan worden toegewezen aan [!UICONTROL Chapek] Corp org omdat deze gebruiker beheerder is van een gekoppeld Analytics-aanmeldingsbedrijf ([!UICONTROL chapek]) en zijn account is gekoppeld aan deze org.
* [!UICONTROL Nigel-prod] Deze gebruiker kan geen verbinding maken met een rapportsuite omdat hij geen beheerder is in een aanmeldingsbedrijf waarvoor deze rapportsuite zichtbaar is.
* [!UICONTROL Doohan-prod] rapportsuite kan worden toegewezen [!UICONTROL Chapek Corp] omdat deze gebruiker een beheerder is van een aanmeldingsbedrijf ([!UICONTROL chapek]) dat is gekoppeld aan de Experience Cloud org (houd er rekening mee dat hij geen beheerder is van het Analytics-aanmeldingsbedrijf van doohan). Het is belangrijk om te weten dat de [!UICONTROL doohan-prod] rapportenreeks ook in aanmerking komt om aan Nigel Inc Experience Cloud org in kaart te worden gebracht, hoewel deze gebruiker niet die afbeelding kan uitvoeren. In dit geval worden beide Experience Cloud-organisaties in de lijst weergegeven, maar [!UICONTROL Nigel Inc] worden ze grijs weergegeven. Voordat de kaart wordt toegewezen, moet deze gebruiker overleg plegen met een beheerder van het nigel-aanmeldingsbedrijf om te bepalen welke org de beste kandidaat is voor mapping. De UI toont een Mogelijke waarschuwing van het Conflict als u een organisatie selecteert is dit verschillend dan de organisatie waaronder de rapportreeks oorspronkelijk werd gecreeerd.

## Veelgestelde vragen {#section_099E485805994C929FF9C9F75219BEE1}

### Waarom zie ik niet al mijn rapportsuites?

Sommige van uw rapportsuites zouden onder een verschillend login bedrijf kunnen zichtbaar zijn. U kunt het huidige login bedrijf veranderen gebruikend drop-down bij de bovenkant van het scherm.

### Wat gebeurt er als ik sommige organisaties die in de vervolgkeuzelijst voor een van mijn rapportensuites zijn vermeld, niet herken?

In de lijst staan alle *mogelijke* organisaties waaraan uw rapportsuite kan worden toegewezen, ook al hebt u geen toestemming om al deze rapportageopets in kaart te brengen. Als u niet zeker weet of de rapportsuite moet worden toegewezen aan een van de grijstinten-uitrapportsuites in de lijst, raadpleegt u een Experience Cloud-beheerder in uw organisatie om de beste keuze te bepalen.

### Wat gebeurt er als ik sommige van de aanmeldingsbedrijven die worden vermeld voor een rapportsuite in de kolom &quot;Zichtbaar voor aanmeldingspartners&quot;, niet herken?

Op een gegeven moment werd deze rapportsuite gedeeld met een ander aanmeldingsbedrijf dat deel kan uitmaken van een andere Experience Cloud-organisatie.

### Wat is deze &quot;Mogelijke Conflict&quot;fout over de rapportreeks die door een andere organisatie wordt geproduceerd? Waarom is dat belangrijk?

Dit is een melding om u te helpen bij het nemen van een geïnformeerde beslissing over de toewijzing van uw rapportsuite. Wij willen u erop wijzen dat de rapportreeks oorspronkelijk onder een verschillende organisatie in het leven werd geroepen voor het geval dat die organisatie voor deze rapportreeks geschikter zou kunnen zijn.

### Hoe weet ik of een rapportenpakket in kaart is gebracht?

Toegewezen rapportsuites worden in een niet-bewerkbare indeling weergegeven. Neem contact op met de klantenservice als u een toewijzing wilt wijzigen.

### Wat als ik alleen de Org ID ken voor mijn Experience Cloud-organisatie? Hoe zoek ik de naam voor mijn Org ID op?

U kunt de naam van uw organisatie vinden in [Organisaties en Accountinstellingen](https://docs.adobe.com/content/help/nl-NL/core-services/interface/manage-users-and-products/organizations.html).

### Ik zie een datum in de kolom &quot;Datum van toewijzing&quot;. Wie heeft dat in kaart gebracht?

U kunt het Logboek van de Verandering van de Reeks van het Rapport in de interface van Analytics raadplegen om de gebruiker te controleren - identiteitskaart die de verandering aanbracht. Zoek naar de gebeurtenis &quot;Suite gekoppeld aan IMS-organisatie&quot;.
