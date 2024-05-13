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
source-git-commit: 0724136e77d6fe1341a64aea75051127956df3b2
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 4%

---

# Organisaties in Experience Cloud

An *organisatie* (Org ID) is de entiteit die een beheerder toelaat om groepen en gebruikers te vormen, en om enig teken-binnen in Experience Cloud te controleren.

De organisatie functioneert als een login bedrijf dat alle producten en toepassingen van het Experience Cloud overspant. Meestal is een organisatie uw bedrijfsnaam. Een bedrijf kan echter veel organisaties hebben.

![Organisaties van Experiencen Cloud](../assets/organizations-menu.png)

Om te controleren dat u zich bij uw correcte organisatie hebt aangemeld, klikt u op uw profielavatar om de naam van de organisatie te zien. Als u toegang hebt tot meer dan één organisatie, kunt u ook een andere organisatie in de kopbalbar bekijken en schakelen.

## Federatieve id&#39;s

Als uw organisatie Federated IDs gebruikt, staat het Experience Cloud u toe om binnen met enige aanmelding van uw organisatie te ondertekenen zonder het worden vereist om uw e-mailadres en wachtwoord in te gaan. Toevoegen `#/sso:@domain` naar de URL van het Experience Cloud (`https://experience.adobe.com`) om deze taak uit te voeren.

Bijvoorbeeld voor een organisatie met federatieve id&#39;s en het domein `adobecustomer.com`, stel uw URL-koppeling in op `https://experience.adobe.com/#/sso:@adobecustomer.com`. U kunt ook rechtstreeks naar een specifieke toepassing gaan door een bladwijzer te maken van deze URL, die bij het toepassingspad wordt gevoegd. (Bijvoorbeeld voor Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Uw organisatie-id weergeven {#concept_EA8AEE5B02CF46ACBDAD6A8508646255}

U kunt uw toegewezen organisatie-id zoeken voor ondersteuningsdoeleinden. U kunt verifiëren dat u in de correcte organisatie bent, of tussen organisaties schakelt, gebruikend **[!UICONTROL Organization]** -menu.

De organisatie-id is de id die is gekoppeld aan uw bedrijf voor het geleverde Experience Cloud. Deze id bestaat uit een alfanumerieke tekenreeks van 24 tekens, gevolgd door (en moet worden opgenomen) `@AdobeOrg`.

U kunt uw organisatie-id samen met andere accountgegevens weergeven met de sneltoets **Ctrl+i** vanaf elke pagina op `https://experience.adobe.com`.

**Uw organisatie-id weergeven**

1. In [Experience Cloud](https://experience.adobe.com), press **Ctrl+i** op uw toetsenbord.

   ![Toegewezen organisatie-id](../assets/assigned-organization.png)

1. Onder **[!UICONTROL User Information]**, zoek naar **[!UICONTROL Current Org ID]** en u kunt de organisatie-id zoeken.

   Beheerders kunnen zich ook aanmelden bij de Admin Console (navigeer naar [https://adminconsole.adobe.com](https://adminconsole.adobe.com)) en bekijk uw organisatie-id in de URL.

   Bijvoorbeeld in de volgende URL:

   `https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

   De id is:

   `C538193582390300A495CC9@AdobeOrg`

## Een toepassingsaccount koppelen aan een Adobe ID {#task_FD389E78640848919E247AC5E95B8369}

Typisch, verlenen de beheerders van het Experience Cloud toegang tot toepassingen en de diensten. In zeldzame gevallen kunt u toepassingsgegevens koppelen aan een Adobe ID.

1. Voer de stappen in uw e-mailuitnodiging voor het Experience Cloud uit.

1. Meld u aan met uw Adobe ID of Enterprise ID.

1. Selecteer de toepassingskiezer. ( ![menu](../assets/menu-icon.png)).

   ![Een toepassingsaccount koppelen aan een Adobe ID](../assets/solutions-active.png)

   De toepassingen waartoe u toegang hebt, zijn gekleurd.

1. Selecteer de gewenste toepassing.

   ![Selecteer de gewenste toepassing](../assets/analytics-link-accounts.png)

   Dit type bericht wordt weergegeven als u deel uitmaakt van de desbetreffende groep (en toestemming hebt voor de toepassing) maar nog geen koppeling hebt gemaakt tussen uw accountgegevens en uw Adobe ID.

1. Selecteren **[!UICONTROL Link Account]** en geef vervolgens uw gegevens op.

## Een standaardorganisatie en -openingspagina opgeven {#concept_6A191B42A9874A9780882903BA18F071}

U kunt een standaardorganisatie en openingspagina opgeven die u wilt gebruiken wanneer u zich aanmeldt.

Selecteer in uw profiel **[!UICONTROL Edit Profile]**.

![Profiel bewerken](../assets/edit-profile.png)

Onder **[!UICONTROL Default Organization & Landing Page]** kunt u uw aanmeldingservaring aanpassen.

![Standaardpagina voor organisatie en landing](../assets/default-organization.png)

## Problemen met het koppelen van accounts oplossen {#concept_DFCB29A3B4834FC59AA29E0BBA301584}

Hulp bij problemen die het gevolg zijn van het koppelen van accounts.

Het koppelen van accounts mislukt doorgaans omdat de Adobe ID is gekoppeld aan een vorige gebruiker. Wanneer het koppelen van een account mislukt, kunt u:

* [Contact opnemen met de Adobe](https://experienceleague.adobe.com/?support-solution=General#support).
* Open uw toepassing met de standaardaanmeldingsnaam terwijl het probleem wordt opgelost.
