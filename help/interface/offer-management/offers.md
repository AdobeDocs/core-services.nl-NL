---
description: Aanbiedingen maken en beheren voor gebruik in Adobe Campaign.
seo-description: Aanbiedingen maken en beheren voor gebruik in Adobe Campaign.
seo-title: Aanbiedingsbeheer
title: Aanbiedingsbeheer
uuid: 83e1d4cd-c5fa-4df0-9603-2914eb4648f8
index: y
translation-type: tm+mt
source-git-commit: a0e0b51d731343d5cd4226ab29d917aca63317c2

---


# Aanbiedingen

Aanbiedingen maken en beheren voor gebruik in Adobe Campaign.

Er zijn twee soorten voorstellen in [!UICONTROL Offer Management]:

| Type | Beschrijving |
|---|---|
| Algemeen aanbod | Hiermee kunt u het volledige gegevensmodel van de aanbieding (geschiktheidsregels, begin- en einddatum en inhoud) invullen. |
| Herkansingsaanbod | De laatste redactie-aanbieding als een klant niet in aanmerking komt voor een van de andere geselecteerde aanbiedingen. U kunt geen toelatingsregels of begin- en einddatums koppelen aan fallback-voorstellen. |

>[!NOTE]
>
>In een aanbiedingsactiviteit, zal u altijd worden gevraagd om een reserveaanbieding te selecteren. Je moet dus ten minste één fallback-aanbieding hebben in je aanbiedingen voordat je een aanbiedingsactiviteit kunt maken.

## Een voorstel maken

Maak een voorstel om het overzicht van je voorstellen aan te vullen.

1. Klik in het [!UICONTROL Inventory] tabblad [!UICONTROL Offer Management]op **[!UICONTROL Create New Offer]** en selecteer **[!UICONTROL Create Offer]**.

   ![](assets/create-offerx.png)

1. Vul de volgende velden in:

   | Veld | Beschrijving |
   |--- |--- |
   | Naam voorstel | De naam die aan de aanbieding is gekoppeld. Je kunt geen twee voorstellen in je voorraad met dubbele namen hebben. |
   | Begindatum | De datum waarop de aanbieding kan worden weergegeven. Als een startdatum van 1/15/17 wordt geselecteerd, kan de aanbieding op 1/15/17 om 12.00 uur beginnen.  Offertebeheer werkt volgens de UTC-tijdstandaard. Dit betekent dat: <ul><li> Aanbiedingen zijn geldig om 00:00 UTC op de dag dat de aanbieding moet beginnen.</li><li> De aanbiedingen verlopen om 00:00 UTC op de dag na de einddatum. Als een aanbieding bijvoorbeeld een einddatum van 5/14 heeft, loopt de aanbieding op 5/15 om 00:00 UTC af. Het aanbod wordt vervolgens gearchiveerd.</li><li>Wanneer e-mails worden voorbereid in Adobe Campaign, worden alleen aanbiedingen weergegeven die op dat moment geldig zijn.</li></ul> |
   | Einddatum | De datum waarop de aanbieding afloopt. Als een einddatum van 20/17 wordt geselecteerd, wordt de aanbieding niet meer weergegeven na 20/17:59 uur. Wanneer een aanbieding zijn einddatum overgaat, wordt het automatisch gearchiveerd. Offertebeheer werkt volgens de UTC-tijdstandaard. Zie de bovenstaande rij voor meer informatie. |
   | Subsidiabiliteitsregels | U kunt toelatingsregels voor aanbiedingen maken op basis van gegevens die beschikbaar zijn in de Campagne-database. De subsidiabiliteitsregels bepalen aan wie en wanneer een aanbieding kan worden getoond.  U kunt bijvoorbeeld opgeven dat u alleen een &#39;Women&#39;s Winter Clothing Offer&#39; wilt laten zien wanneer (Gender = &#39;Vrouwelijk&#39;) en (Region = &#39;Noordoost&#39;). De attributen die worden gebruikt om deze regels te bouwen komen uit het profiel van de Norm van de Campagne.  Opmerking:  Wanneer u eerst tot het Beheer van de Aanbieding toegang hebt, zijn er geen attributen beschikbaar in de regelbouwer. U moet kenmerken van de campagne-interface delen. Zodra gedeeld, zijn die attributen beschikbaar. |
   | Max. uiteinde | De maximumtijden die een aanbieding kan worden voorgesteld.  Opmerking:  Het aantal keren dat een aanbieding wordt voorgesteld, wordt berekend tijdens de voorbereiding van e-mail. Als u bijvoorbeeld een e-mail met een aantal voorstellen voorbereidt, tellen deze nummers mee voor de maximale limiet, ongeacht of de e-mail is verzonden of niet. |
   | Maximale limiet per gebruiker | De maximumtijden dat een aanbieding aan een bepaalde gebruiker kan worden voorgesteld.  Opmerking:  Het aantal keren dat een aanbieding aan een bepaalde gebruiker wordt voorgesteld, wordt berekend bij de voorbereiding van e-mail. Als u bijvoorbeeld een e-mail met een aantal voorstellen voorbereidt, tellen deze nummers mee voor de maximale limiet per gebruiker, ongeacht of de e-mail al dan niet is verzonden. |
   | Labels | Voeg labels toe aan een aanbieding om ze samen te groeperen. U kunt typen en op Enter drukken om een nieuw label te maken of beginnen te typen en een bestaand aanbod te selecteren in de vervolgkeuzelijst. |

1. Vul de weergavedetails in.

   | Veld | Beschrijving |
   |---|---|
   | Kanaal | Het kanaal waarin deze inhoudsrepresentatie kan worden geleverd. E-mails over de standaard voor campagnes zijn momenteel het enige kanaal dat beschikbaar is. |
   | Plaatsing | Selecteer de plaatsing waarin deze inhoudsrepresentatie kan worden geleverd. Plaatsen worden vooraf ingevuld op het tabblad Plaatsen. U moet elke inhoudsrepresentatie koppelen aan een plaatsing in het keuzemenu. U kunt geen meerdere inhoudsrepresentaties maken met dezelfde plaatsing in dezelfde aanbieding. |
   | Inhoudstype | Selecteer een inhoudstype van een afbeelding, afbeelding-URL, tekst of HTML. |
   | Koppeling omleiden | Dit veld wordt weergegeven als u een inhoudstype van de URL van de afbeelding of afbeelding selecteert. Dit is de koppeling waarnaar de gebruiker wordt omgeleid als hij of zij op die aanbieding in een e-mail klikt. |

1. Klik **[!UICONTROL Save & Preview]** om de details van je voorstel te bekijken voordat je het verzendt.
1. Klik **[!UICONTROL Approve]** om het voorstel goed te keuren. Zodra de aanbieding in de goedgekeurde staat is, kan het in een aanbiedingsactiviteit worden gebruikt.

   Als u niet de vereiste toestemmingen hebt om een aanbieding goed te keuren, zult u in plaats daarvan klikken **[!UICONTROL Submit]**. De aanbieding wordt dan weergegeven in de aanbiedingsbibliotheek met een status die in behandeling is. Zodra een gebruiker met goedkeuringsrechten het goedkeurt, zal het voor gebruik in een aanbiedingsactiviteit beschikbaar zijn.
