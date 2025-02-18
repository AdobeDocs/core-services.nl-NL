---
description: Meer informatie over organisaties (IMS-organisatie-ID) en het koppelen van oplossingsaccounts aan Experience Cloud.
solution: Experience Cloud
title: Organisaties en account koppelen
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Organizations
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
source-git-commit: 1e0206286d4ac0f1987ee053bcbfce8649902ccd
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 4%

---

# Organisaties in Experience Cloud

Een *organisatie* (Org identiteitskaart) is de entiteit die een beheerder toelaat om groepen en gebruikers te vormen, en enig teken-binnen in Experience Cloud te controleren.

De organisatie werkt als een login bedrijf dat alle producten en toepassingen van Experience Cloud overspant. Meestal is een organisatie uw bedrijfsnaam. Een bedrijf kan echter veel organisaties hebben.

![ de Organisaties van Experience Cloud ](../assets/organizations-menu.png)

Als u wilt controleren of u zich hebt aangemeld bij de juiste organisatie, klikt u op **[!UICONTROL Profile]** om de standaardorganisatienaam weer te geven. Als u toegang hebt tot meer dan één organisatie, kunt u ook een andere organisatie in de kopbalbar bekijken en schakelen.

## Federatieve id&#39;s

Als uw organisatie Federated IDs gebruikt, staat Experience Cloud u toe om binnen met enige aanmelding van uw organisatie te ondertekenen zonder het worden vereist om uw e-mailadres en wachtwoord in te gaan. Voeg `#/sso:@domain` aan Experience Cloud URL (`https://experience.adobe.com`) toe om deze taak te verwezenlijken.

Stel bijvoorbeeld voor een organisatie met federatieve id&#39;s en het domein `adobecustomer.com` de URL-koppeling in op `https://experience.adobe.com/#/sso:@adobecustomer.com` . U kunt ook rechtstreeks naar een specifieke toepassing gaan door een bladwijzer te maken van deze URL, die bij het toepassingspad wordt gevoegd. (Bijvoorbeeld voor Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics` .)

## Uw organisatie-id weergeven {#concept_EA8AEE5B02CF46ACBDAD6A8508646255}

U kunt uw toegewezen organisatie-id zoeken voor ondersteuningsdoeleinden. Met de kiezer **[!UICONTROL Organization]** in de header kunt u controleren of u zich in de juiste organisatie bevindt of kunt u schakelen tussen organisaties.

De organisatie-id is de id die aan uw Experience Cloud-bedrijf is toegewezen. Deze id is een alfanumerieke tekenreeks van 24 tekens, gevolgd door (en moet omvatten) `@AdobeOrg` .

U kunt uw organisatieidentiteitskaart, samen met andere rekeningsinformatie bekijken, gebruikend de toetsenbordkortere weg **Ctrl+i** van om het even welke pagina bij `https://experience.adobe.com`.

**om uw organisatieidentiteitskaart** te bekijken

1. In [ Experience Cloud ](https://experience.adobe.com), druk **Ctrl+i** op uw toetsenbord.

   ![ Toegewezen identiteitskaart van de Organisatie ](../assets/assigned-organization.png)

1. Ga naar **[!UICONTROL Current Org ID]** onder **[!UICONTROL User Information]** en zoek de organisatie-id.

   Alternatief, kunnen de beheerders in Admin Console (navigeer aan [ https://adminconsole.adobe.com ](https://adminconsole.adobe.com)) registreren en uw organisatieidentiteitskaart in URL bekijken.

   Bijvoorbeeld in de volgende URL:

   `https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

   De id is:

   `C538193582390300A495CC9@AdobeOrg`

## Een toepassingsaccount koppelen aan een Adobe ID {#task_FD389E78640848919E247AC5E95B8369}

Experience Cloud-beheerders verlenen doorgaans toegang tot toepassingen en services. In zeldzame gevallen kunt u toepassingsgegevens koppelen aan een Adobe ID.

1. Voer de stappen in uw e-mailuitnodiging voor Experience Cloud uit.

1. Meld u aan met uw Adobe ID of Enterprise ID.

1. Klik op **[!UICONTROL Application selector]** . ( ![ menu ](../assets/apps-icon.png)).

   ![ Verbinding een toepassingsrekening aan een Adobe ID ](../assets/solutions-active.png)

   De toepassingen waartoe u toegang hebt, zijn gekleurd.

1. Klik op de gewenste toepassing.

   ![ klik uw toepassing ](../assets/analytics-link-accounts.png)

   Dit type bericht wordt weergegeven als u deel uitmaakt van de desbetreffende groep (en toestemming hebt voor de toepassing) maar nog geen koppeling hebt gemaakt tussen uw accountgegevens en uw Adobe ID.

1. Klik op **[!UICONTROL Link Account]** en geef vervolgens uw referenties op.

## Een standaardorganisatie opgeven {#concept_6A191B42A9874A9780882903BA18F071}

U kunt een standaardorganisatie opgeven die moet worden gebruikt wanneer u zich aanmeldt.

1. Klik in de koptekst op **[!UICONTROL Profile]** en klik vervolgens op Voorkeuren.

1. Selecteer onder [!UICONTROL General] een standaardorganisatie.


![ geef Profiel ](../assets/edit-profile.png) uit

## Problemen met het koppelen van accounts oplossen {#concept_DFCB29A3B4834FC59AA29E0BBA301584}

Hulp bij problemen die het gevolg zijn van het koppelen van accounts.

Het koppelen van accounts mislukt doorgaans omdat de Adobe ID is gekoppeld aan een vorige gebruiker. Wanneer het koppelen van een account mislukt, kunt u:

* [ de Steun van Adobe van het Contact ](https://experienceleague.adobe.com/?support-solution=General#support).
* Open uw toepassing met de standaardaanmeldingsnaam terwijl het probleem wordt opgelost.
