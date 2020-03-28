---
description: Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.
seo-description: Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.
seo-title: Kaart rapportsuites aan een organisatie
title: Kaart rapportsuites aan een organisatie
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Kaart rapportsuites aan een organisatie {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Leer hoe u een of meerdere rapportreeksen aan een organisatie toewijst.

De diensten van de Wolk van de ervaring (zoals de Dienst van identiteitskaart van de Ervaring Cloud en de de kerndienst van Mensen) worden geassocieerd met een organisatie in plaats van een individuele rapportreeks. Om ervoor te zorgen dat deze services correct werken, moet elke analytische rapportensuite aan een organisatie worden toegewezen. Het toewijzingsproces:

* Stelt een Experience Cloud-organisatie in als de primaire organisatie voor de rapportsuite.
* Hiermee wordt niet gewijzigd wie toegang heeft tot een rapportsuite (de toegang wordt nog steeds bepaald door de Adobe Analytics-aanmeldingsaccount voor elke gebruiker)

## Vereisten

U moet een beheerder van Analytics van een login bedrijf zijn dat toegang tot de rapportreeks heeft u wilt in kaart brengen. Bovendien moet deze account zijn [gekoppeld aan een Experience Cloud-organisatie](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) om de rapportreeksen aan die organisatie toe te wijzen.

Organisaties worden grijs weergegeven als u geen beheerdersmachtigingen voor Analytics hebt voor een aanmeldingsbedrijf onder die organisatie die toegang heeft tot de opgegeven rapportsuite.

## Een rapportsuite toewijzen aan een organisatie {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Klik op **[!UICONTROL Experience Cloud]** > **[!UICONTROL Beheer]** > **[!UICONTROL Reeks toewijzen rapporteren]**

1. Om de login bedrijven te zien die toegang tot elke rapportreeks hebben, klik **[!UICONTROL Zichtbaar aan Login Bedrijven]**.

   Deze mening is bedoeld om u te helpen een geïnformeerde beslissing over de afbeelding nemen.

1. Klik de drop-down in de **[!UICONTROL Toegewezen kolom van de Organisatie]** naast een rapportreeks en selecteer de organisatie waaraan u wilt in kaart brengen.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

## Meerdere rapportsuites toewijzen aan een organisatie {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Klik op **[!UICONTROL Experience Cloud]** > **[!UICONTROL Beheer]** > **[!UICONTROL Reeks toewijzen]** rapporteren.

1. Selecteer de rapportsuites die u wilt in kaart brengen.

   ![](assets/rs-mapping-multiple.png)

1. Selecteer de organisatie (Outdoor Inc, in dit voorbeeld), dan klik **[!UICONTROL Uitgezocht]**.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

1. Klik op Toewijzing **[!UICONTROL opslaan]**.

## Tips voor het selecteren van een Experience Cloud Organization {#mapping-tips}

Deze sectie bevat tips voor het selecteren van de Experience Cloud-organisatie waaraan u een rapportsuite moet toewijzen.

### Welke organisatie moet ik kiezen?

Als de Experience Cloud ID Service momenteel wordt geïmplementeerd in de rapportsuite, moet u ervoor zorgen dat de organisatie die u selecteert in het hulpprogramma voor het toewijzen van de rapportsuite dezelfde organisatie is als die is opgegeven in het [!DNL visitorAPI.js] bestand op uw site. U kunt de instructies in de [Test gebruiken en de dienst](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) van identiteitskaart van de Wolk verifiëren van de Ervaring om org identiteitskaart te vinden die door de dienst van identiteitskaart van de Bezoeker wordt gebruikt.

Als de dienst van identiteitskaart van de Bezoeker nog niet op de plaatsen wordt opgesteld die gegevens voor de rapportreeks verzamelen, als u de dienst van identiteitskaart van de Bezoeker van de Wolk van de Ervaring in de toekomst opstelt, zult u moeten verzekeren uw plaatsing de organisatie aanpast u in het hulpmiddel van de Afbeelding van de Reeks van het Rapport koos.

### Waarom worden sommige organisaties gegraveerd?

Dit wijst erop dat u niet genoeg voorrechten hebt om aan de grayed-uit rapportreeks in kaart te brengen. Bekijk het volgende voorbeeld:

![](assets/rs-mapping.png)

In dit diagram geeft de blauwe sleutel beheerdersrechten aan. De grijze lijnen geven de zichtbaarheid aan.

Deze gebruiker heeft toegang tot twee Experience Cloud-organisaties. Hij heeft het volgende gedaan:

* Koppelde zijn beheerdersaccount in het [!UICONTROL chapek] Analytics-aanmeldingsbedrijf aan zijn [!UICONTROL Chapek] Corp Experience Cloud-organisatieaccount.
* Koppelde zijn niet-beheerdersaccount in het [!UICONTROL doohan] Analytics-aanmeldingsbedrijf aan zijn [!UICONTROL Chapek] Corp Experience Cloud-organisatieaccount.
* Koppelde zijn niet-beheerdersaccount in de inlognaam nigel Analytics aan zijn Nigel Inc Experience Cloud org-account.

De volgende punten geven een overzicht van de toewijzingsacties die deze gebruiker kan en kan uitvoeren met betrekking tot deze rapportsuites:

* [!UICONTROL Chapek-prod] rapportsuite kan worden toegewezen aan [!UICONTROL Chapek] Corp org omdat deze gebruiker beheerder is van een gekoppeld Analytics-aanmeldingsbedrijf ([!UICONTROL chapek]) en zijn account is gekoppeld aan deze org.
* [!UICONTROL Nigel-prod] rapportenreeks kan niet door deze gebruiker worden verbonden aangezien hij geen beheerder in om het even welk login bedrijf is waaraan deze rapportreeks zichtbaar is.
* [!UICONTROL De Doohan-prod] rapportsuite kan worden toegewezen aan [!UICONTROL Chapek Corp] , aangezien deze gebruiker een beheerder is van een aanmeldingsbedrijf ([!UICONTROL chapek]) dat is gekoppeld aan de Experience Cloud org (houd er rekening mee dat hij geen beheerder is van het aanmeldingsbedrijf van Dohan Analytics). Het is belangrijk om te weten dat de [!UICONTROL doohan-prod] rapportenreeks ook in aanmerking komt om aan de Nigel Inc Experience Cloud org in kaart te worden gebracht, ook al kan deze gebruiker die afbeelding niet uitvoeren. In dit geval worden beide Experience Cloud-organisaties weergegeven in de lijst, maar [!UICONTROL Nigel Inc] wordt grijs weergegeven. Voordat de kaart wordt toegewezen, moet deze gebruiker overleg plegen met een beheerder van het nigel-aanmeldingsbedrijf om te bepalen welke org de beste kandidaat is voor mapping. De UI toont een Mogelijke waarschuwing van het Conflict als u een organisatie selecteert is dit verschillend dan de organisatie waaronder de rapportreeks oorspronkelijk werd gecreeerd.

## Frequently Asked Questions {#section_099E485805994C929FF9C9F75219BEE1}

### Waarom zie ik niet al mijn rapportsuites?

Sommige van uw rapportsuites zouden onder een verschillend login bedrijf kunnen zichtbaar zijn. U kunt het huidige login bedrijf veranderen gebruikend drop-down bij de bovenkant van het scherm.

### Wat gebeurt er als ik sommige organisaties die in de vervolgkeuzelijst voor een van mijn rapportensuites zijn vermeld, niet herken?

In de lijst staan alle *mogelijke* organisaties waaraan uw rapportsuite kan worden toegewezen, ook al hebt u geen toestemming om al deze rapportageopets in kaart te brengen. Als u niet zeker weet of de rapportsuite moet worden toegewezen aan een van de grijstinten-uitrapportsuites in de lijst, raadpleegt u een beheerder van de Experience Cloud in uw organisatie om de beste keuze te bepalen.

### Wat gebeurt er als ik sommige van de aanmeldingsbedrijven die worden vermeld voor een rapportsuite in de kolom &quot;Zichtbaar voor aanmeldingspartners&quot;, niet herken?

Op een gegeven moment werd deze rapportsuite gedeeld met een ander aanmeldingsbedrijf dat deel kan uitmaken van een andere Experience Cloud-organisatie.

### Wat is deze &quot;Mogelijke Conflict&quot;fout over de rapportreeks die door een andere organisatie wordt geproduceerd? Waarom is dat belangrijk?

Dit is een melding om u te helpen bij het nemen van een geïnformeerde beslissing over de toewijzing van uw rapportsuite. Wij willen u erop wijzen dat de rapportreeks oorspronkelijk onder een verschillende organisatie in het leven werd geroepen voor het geval dat die organisatie voor deze rapportreeks geschikter zou kunnen zijn.

### Hoe weet ik of een rapportenpakket in kaart is gebracht?

Toegewezen rapportsuites worden in een niet-bewerkbare indeling weergegeven. Neem contact op met de klantenservice als u een toewijzing wilt wijzigen.

### Wat gebeurt er als ik alleen de Org ID ken voor mijn Experience Cloud-organisatie? Hoe zoek ik de naam van mijn Org ID op?

U kunt de naam van uw organisatie vinden in [Organisaties en Accountinstellingen](https://docs.adobe.com/content/help/en/core-services/interface/manage-users-and-products/organizations.html).

### Ik zie een datum in de kolom &quot;Datum van toewijzing&quot;. Wie heeft dat in kaart gebracht?

U kunt het Logboek van de Verandering van de Reeks van het Rapport in de interface van Analytics raadplegen om gebruiker te controleren - identiteitskaart die de verandering aanbracht. Zoek naar de gebeurtenis &quot;Suite gekoppeld aan IMS-organisatie&quot;.
