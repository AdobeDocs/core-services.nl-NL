---
description: Meer informatie over organisaties en het koppelen van oplossingsaccounts aan Experience Cloud.
keywords: Adobe Experience Cloud-services
solution: Experience Cloud
title: 'Organisaties en accountkoppelingen '
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
source-git-commit: ec724555c3799eeca350592498267d0b71b4ff04
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 6%

---

# Organisaties in Experience Cloud

Leer over het beheren van en het schakelen van organisaties in Experience Cloud.

## Uw organisatie identificeren {#concept_384D169B0B724B799D573B8ECB5C39BF}

Een *organisatie* is de entiteit die een beheerder toelaat om groepen en gebruikers te vormen, en enig teken-binnen in de Experience Cloud te controleren. De organisatie functioneert als een aanmeldingsbedrijf dat alle producten en oplossingen van Experience Cloud omvat. Meestal is een organisatie uw bedrijfsnaam. Een bedrijf kan echter vele organisaties hebben.

Om te controleren dat u zich bij uw correcte organisatie hebt aangemeld, klikt u op uw profielavatar om de naam van de organisatie te zien. Als u toegang hebt tot meer dan één organisatie, kunt u ook bekijken en op een andere organisatie in de kopbalbar schakelen.

Als uw organisatie Federated IDs gebruikt, staat Experience Cloud u toe om binnen met enige aanmelding van uw organisatie te ondertekenen zonder de behoefte om uw e-mailadres en wachtwoord in te gaan. Om dit te doen, voeg `#/sso:@domain` aan Experience Cloud URL (`https://experience.adobe.com`) toe.

Stel bijvoorbeeld voor een organisatie met Federatieve id&#39;s en het domein `adobecustomer.com` de URL-koppeling in op `https://experience.adobe.com/#/sso:@adobecustomer.com`. U kunt ook rechtstreeks naar een specifieke toepassing gaan door een bladwijzer te maken van deze URL, die bij het toepassingspad wordt gevoegd. (Voor Adobe Analytics bijvoorbeeld `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

![Stap Resultaat](assets/organization-switch.png)

## Zoek uw organisatie-id {#concept_EA8AEE5B02CF46ACBDAD6A8508646255}

Mogelijk moet u uw organisatie-id zoeken voor ondersteuningsdoeleinden. Met het menu **[!UICONTROL Organization]** kunt u controleren of u zich in de juiste organisatie bevindt of kunt u schakelen tussen organisaties.

De **organisatie-id** is de id die is gekoppeld aan uw ingeleverde Experience Cloud-bedrijf. Deze id is een alfanumerieke tekenreeks van 24 tekens, gevolgd door (en moet bevatten) @AdobeOrg.

Als u uw organisatie-id wilt weergeven, navigeert u naar de bestemmingspagina van de Experience Cloud of selecteert u ( ![](assets/menu-icon.png)) en selecteert u **[!UICONTROL Administration]**. U vindt de organisatie-id onder aan de pagina [!UICONTROL Getting Started with the Experience Cloud] of op de pagina [!UICONTROL Administration].

![](assets/administration-page.png)

## Een oplossingsaccount koppelen aan een Adobe ID {#task_FD389E78640848919E247AC5E95B8369}

Typisch, verlenen de beheerders van Experience Cloud toegang tot oplossingen en de diensten. In zeldzame omstandigheden, kunt u oplossingsgeloofsbrieven aan een Adobe ID moeten verbinden.

1. Voer de stappen in uw e-mailuitnodiging voor de Experience Cloud uit.
1. Meld u aan met uw Adobe ID of Enterprise ID.
1. Selecteer de oplossingenkiezer. ( ![](assets/menu-icon.png)).

   ![](assets/solutions-active.png)

   De oplossingen waartoe u toegang hebt, zijn gekleurd.
1. Selecteer de gewenste oplossing.

   ![](assets/analytics-link-accounts.png)

   Dit type bericht wordt weergegeven als u deel uitmaakt van de desbetreffende groep (en toestemming hebt voor de oplossing) maar uw accountgegevens nog niet aan uw Adobe ID hebt gekoppeld.
1. Selecteer **[!UICONTROL Link Account]** en geef uw referenties op.

## Een standaardorganisatie en -openingspagina opgeven {#concept_6A191B42A9874A9780882903BA18F071}

U kunt een standaardorganisatie en openingspagina opgeven die u wilt gebruiken wanneer u zich aanmeldt.

Selecteer **[!UICONTROL Edit Profile]** in uw profiel.

![](assets/edit-profile.png)

Bij Standaardorganisatie en -bestemmingspagina kunt u uw aanmeldingservaring aanpassen.

![](assets/default-organization.png)

## Problemen met koppelingen tussen accounts oplossen {#concept_DFCB29A3B4834FC59AA29E0BBA301584}

Hulp bij problemen die het gevolg zijn van het koppelen van accounts.

Het koppelen van accounts mislukt doorgaans omdat de Adobe ID is gekoppeld aan een vorige gebruiker. Wanneer het koppelen van een account mislukt, kunt u:

* [Neem contact op met de Adobe-ondersteuning](https://experienceleague.adobe.com/?support-solution=General#support).
* Heb toegang tot uw oplossing gebruikend standaardlogin terwijl de kwestie wordt opgelost.
