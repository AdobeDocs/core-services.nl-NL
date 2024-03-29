---
description: Leer hoe u een of meerdere rapportsuites toewijst aan een organisatie in Experience Cloud.
title: 'Kaart rapportsuites aan een organisatie '
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 4e9f0f7a-8e16-4473-af4a-3e74ad50c044
source-git-commit: c073b3bacf5505c01017d4ba2507621df8ef877e
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# Kaart rapportsuites aan een organisatie {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

>[!NOTE]
>
>De functie voor het toewijzen van rapportsuite is in november 2020 afgekeurd. Neem contact op met de Klantenondersteuning voor alle vragen.

Experience Cloud-services (zoals Experience Cloud ID-service en [!UICONTROL People]) zijn gekoppeld aan een organisatie in plaats van aan een afzonderlijke rapportsuite. Om ervoor te zorgen dat deze services correct werken, moet elke analytische rapportensuite aan een organisatie worden toegewezen. Het toewijzingsproces:

* Plaatst een organisatie van de Experience Cloud als primaire organisatie voor de rapportreeks.
* Wijzigt niet wie toegang heeft tot een rapportsuite (de toegang wordt nog steeds bepaald door de Adobe Analytics-aanmeldingsaccount voor elke gebruiker)

## Vereisten

U moet een beheerder van Analytics van een login bedrijf zijn dat toegang tot de rapportreeks heeft u wilt in kaart brengen. Deze account moet ook [verbonden met een Experience Cloud-organisatie](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) om aan die organisatie rapporteringssuites toe te wijzen.

Organisaties worden grijs weergegeven als u geen beheerdersmachtigingen voor Analytics hebt voor een aanmeldingsbedrijf onder die organisatie die toegang heeft tot de opgegeven rapportsuite.

## Een rapportsuite toewijzen aan een organisatie {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Navigeer naar Rapporten Suites voor gegevensbeheer bij [!DNL Analytics] > **[!UICONTROL Admin]** > **[!UICONTROL Data Governance]** (zie [De instelling voor gegevensbeheer van de rapportsuite weergeven/beheren](https://experienceleague.adobe.com/docs/analytics/admin/data-governance/gdpr-view-settings.html?lang=en)

1. Om de login bedrijven te zien die toegang tot elke rapportreeks hebben, selecteer **[!UICONTROL Visible to Login Companies]**.

   Deze mening is bedoeld om u te helpen een geïnformeerde beslissing over de afbeelding nemen.

1. Selecteer de vervolgkeuzelijst in het dialoogvenster **[!UICONTROL Mapped Organization]** kolom naast een rapportreeks en selecteer de organisatie waaraan u wilt in kaart brengen.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

## Meerdere rapportsuites toewijzen aan een organisatie {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Selecteer **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**.

1. Selecteer de rapportsuites die u wilt in kaart brengen.

   ![Selecteer de rapportsuites die u wilt in kaart brengen](assets/rs-mapping-multiple.png)

1. Selecteer de organisatie (Outdoor Inc, in dit voorbeeld), dan klik **[!UICONTROL Select]**.

   Zie de volgende sectie voor tips over het selecteren van een Experience Cloud-organisatie.

1. Selecteer **[!UICONTROL Save Mapping]**.

## Tips voor het selecteren van een Experience Cloud-organisatie {#mapping-tips}

Deze sectie bevat uiteinden om u te helpen de organisatie van de Experience Cloud selecteren waaraan u een rapportreeks in kaart zou moeten brengen.

### Welke organisatie moet ik kiezen?

Als de Experience Cloud-id-service wordt geïmplementeerd in de rapportsuite, moet u ervoor zorgen dat de organisatie die u selecteert in het gereedschap voor het toewijzen van de rapportsuite dezelfde organisatie is als in het dialoogvenster [!DNL visitorAPI.js] op uw site. U kunt de instructies in [De Experience Cloud ID-service testen en controleren](https://experienceleague.corp.adobe.com/docs/id-service/using/implementation/test-verify.html) om de org-id te zoeken die wordt gebruikt door de service Bezoeker-id.

Zorg ervoor dat uw implementatie overeenkomt met de organisatie die u hebt gekozen in het hulpprogramma voor het toewijzen van de rapportsuite.

### Waarom worden sommige organisaties gegraveerd?

Het oppakken van een organisatie wijst erop dat u niet voldoende voorrechten hebt om aan de grayed-uit rapportreeks in kaart te brengen. Bekijk het volgende voorbeeld:

![Waarom worden sommige organisaties gegraveerd?](assets/rs-mapping.png)

In dit diagram geeft de blauwe sleutel beheerdersrechten aan. De grijze lijnen geven de zichtbaarheid aan.

Deze gebruiker heeft toegang tot twee organisaties van de Experience Cloud. Zij hebben het volgende uitgevoerd:

* Hun beheerdersaccount is gekoppeld in het dialoogvenster [!UICONTROL chapek] Logboekbedrijf van Analytics aan hun [!UICONTROL Chapek] Organisatierekening van Corp Experience Cloud.
* Hun niet-beheerdersaccount is gekoppeld in het dialoogvenster [!UICONTROL doohan] Logboekbedrijf van Analytics aan hun [!UICONTROL Chapek] Organisatierekening van Corp Experience Cloud.
* Koppelde hun niet-beheerdersaccount in de inlognaam nigel Analytics aan hun Nigel Inc Experience Cloud org-account.

De volgende punten geven een overzicht van de toewijzingsacties die deze gebruiker kan en kan uitvoeren met betrekking tot deze rapportsuites:

* [!UICONTROL Chapek-prod] rapportsuite kan worden toegewezen aan [!UICONTROL Chapek] Corp org omdat deze gebruiker beheerder is van een gekoppeld Analytics-aanmeldingsbedrijf ([!UICONTROL chapek]) en zijn account is gekoppeld aan deze org.
* [!UICONTROL Nigel-prod] Deze gebruiker kan geen verbinding maken met de rapportsuite omdat deze geen beheerder is in een aanmeldingsbedrijf waarvoor deze rapportsuite zichtbaar is.
* [!UICONTROL Doohan-prod] rapportsuite kan worden toegewezen aan [!UICONTROL Chapek Corp] aangezien deze gebruiker een beheerder van een login bedrijf is ([!UICONTROL chapek]) die is gekoppeld aan de Experience Cloud org (merk op dat hij geen beheerder is van het aanmeldingsbedrijf van doohan Analytics). Het is belangrijk te weten dat de [!UICONTROL doohan-prod] rapportsuite komt ook in aanmerking om te worden toegewezen aan Nigel Inc Experience Cloud org, ook al kan deze gebruiker die toewijzing niet uitvoeren. In dit geval worden beide Experience Cloud-organisaties weergegeven in de lijst, maar [!UICONTROL Nigel Inc] is grijs. Voordat de kaart wordt toegewezen, moet deze gebruiker overleg plegen met een beheerder van het nigel-aanmeldingsbedrijf om te bepalen welke org de beste kandidaat is voor mapping. De UI toont een Mogelijke waarschuwing van het Conflict als u een organisatie selecteert is dit verschillend van de organisatie waaronder de rapportreeks oorspronkelijk werd gecreeerd.

## Veelgestelde vragen {#section_099E485805994C929FF9C9F75219BEE1}

### Waarom zie ik niet al mijn rapportsuites?

Sommige van uw rapportsuites zouden onder een verschillend login bedrijf kunnen zichtbaar zijn. U kunt het huidige login bedrijf veranderen gebruikend drop-down bij de bovenkant van het scherm.

### Wat gebeurt er als ik sommige organisaties die in de vervolgkeuzelijst voor een van mijn rapportensuites zijn vermeld, niet herken?

In de lijst worden alle *mogelijk* organisaties waaraan uw rapportsuite kan worden toegewezen, zelfs als u geen toestemming hebt om aan al die rapportsuites toe te wijzen. Als u niet zeker bent of de rapportreeks aan één van grayed-uit rapportreeksen in de lijst zou moeten worden in kaart gebracht, gelieve een beheerder van de Experience Cloud in uw organisatie te raadplegen om de beste keus te bepalen.

### Wat gebeurt er als ik sommige van de aanmeldingsbedrijven die worden vermeld voor een rapportsuite in de kolom &quot;Zichtbaar voor aanmeldingspartners&quot;, niet herken?

Op een gegeven moment werd deze rapportsuite gedeeld met een ander aanmeldingsbedrijf dat deel kan uitmaken van een andere Experience Cloud-organisatie.

### Wat is deze &quot;Mogelijke Conflict&quot;fout over de rapportreeks die door een andere organisatie wordt geproduceerd? Waarom is dat belangrijk?

Met deze melding kunt u een geïnformeerde beslissing nemen over de toewijzing van de rapportsuite. Wij willen u erop wijzen dat de rapportreeks oorspronkelijk onder een verschillende organisatie in het leven werd geroepen voor het geval dat die organisatie voor deze rapportreeks geschikter zou kunnen zijn.

### Hoe weet ik of een rapportenpakket in kaart is gebracht?

Toegewezen rapportsuites worden getoond in een niet-editable formaat. Neem contact op met de klantenservice als u een toewijzing moet wijzigen.

### Wat als ik alleen de Org-id ken voor mijn Experience Cloud-organisatie? Hoe zoek ik de naam voor mijn Org ID op?

U kunt de naam van uw organisatie vinden in [Organisaties en accountinstellingen](organizations.md).

### Ik zie een datum in de kolom &quot;Datum van toewijzing&quot;. Wie heeft dat in kaart gebracht?

U kunt het Logboek van de Verandering van de Reeks van het Rapport in de interface van Analytics raadplegen om gebruiker te controleren - identiteitskaart die de verandering aanbracht. Zoek naar de gebeurtenis &quot;Suite gekoppeld aan IMS-organisatie&quot;.
