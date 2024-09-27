---
title: Accountvoorkeuren en -meldingen
description: Meer informatie over gebruikersprofielen en accountvoorkeuren in Experience Cloud. Abonneren op productmeldingen voor e-mail en  [!DNL Slack] en productwaarschuwingen instellen.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: 9a6833139a0fb8eed8a10daeda34f354a7133f17
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# Accountvoorkeuren en -meldingen {#preferences}

Om de voorkeur van het Experience Cloud te vinden, klik uw **[!UICONTROL User Account]** ![ voorkeur ](../assets/preferences-icon-sm.png) pictogram in de kopbal, dan klik **[!UICONTROL Preferences]**.

![ voorkeur ](../assets/preferences-navigation.png){width="100" zoomable="yes"}

Op de pagina [!UICONTROL Experience Cloud preferences] kunt u de volgende accountfuncties beheren:

| Functie | Beschrijving |
|--- |--- |
| Profiel | Werk uw [ Profiel van de Rekening van de Adobe ](https://account.adobe.com/profile) bij. <p>Uw profielfoto en naam worden weergegeven wanneer u zich aanmeldt bij Adobe.com, producten en services van de Adobe opneemt en op openbare sites zoals [!DNL Behance] . |
| Algemeen | Selecteer een [ organisatie ](../administration/organizations.md).<p>Dit is de standaardorganisatie die wordt gebruikt wanneer u zich aanmeldt bij een Experience Cloud. |
| [!UICONTROL Product data collection] | Selecteer welke technologieën Adobe kan gebruiken om gegevens te verzamelen over hoe u uw producten van de Adobe gebruikt. |
| Meldingen | Vorm hoe en wanneer u product [ berichten ](#subscribe-to-notifications-in-experience-cloud) en alarm zou willen: <ul><li>Selecteer de producten waarop u zich wilt abonneren voor waarschuwingen</li><li>Vorm het type van bericht ([!UICONTROL in-app], [!UICONTROL email], of [ Slack ](#slack-notifications))</li><li>Geef de frequentie op waarmee je e-mailberichten wilt ontvangen. (Niet verzonden, onmiddellijk, dagelijks of wekelijks.)</li><li>Bepaal de waakzame prioriteit. In-app-waarschuwingen worden een paar seconden in de rechterbovenhoek van uw venster weergegeven. U kunt ook opgeven of waarschuwingen moeten worden weergegeven totdat u ze verwijdert.</li></ul> |
| [!UICONTROL Personalized learning recommendations and promotions] | Selecteer waar u [ gepersonaliseerde hulp ](personalized-learning.md) voor uw producten van de Adobe zou willen ontvangen. Deze Help is beschikbaar via e-mail, in-product, en de Gemeenschappen van de Experience League. |

## Abonneren op meldingen in Experience Cloud {#notifications}

Je kunt de producten en rubrieken selecteren waarop je je wilt abonneren. De berichten verschijnen in [!UICONTROL Notifications] popover (in-app), of in uw e-mail, of in [ Slack ](#slack-notifications) (afhankelijk van uw abonnementen).

Meldingen via e-mail en Slack zijn handig voor situaties waarin u niet bent aangemeld bij Experience Cloud.

### Abonneren op in-app- en e-mailmeldingen

1. Navigeer aan Experience Cloud [ voorkeur ](https://experience.adobe.com/preferences).

1. Schakel onder **[!UICONTROL Notifications]** **[!UICONTROL In-app]** of **[!UICONTROL Email]** in.

   Wijzigingen in meldingen worden automatisch opgeslagen.

### Abonneren op [!DNL Slack] meldingen {#slack}

U kunt uw accountvoorkeuren zo configureren dat meldingen van Experiencen Cloud naar een [!DNL Slack] -kanaal worden verzonden.

**Vereisten**

* Je moet een Experience Cloud account hebben.
* U moet een [!DNL Slack] account hebben. Uw [!DNL Slack] -beheerder schakelt de integratie van het Experience Cloud met [!DNL Slack] in.
* U moet onderdeel zijn van ten minste één [!DNL Slack] -werkruimte.

**om aan [!DNL Slack] berichten** in te schrijven

1. Navigeer aan Experience Cloud [ Voorkeur ](https://experience.adobe.com/preferences).

1. Zoek [!DNL Slack] en klik vervolgens op **[!UICONTROL Add to Slack]** .

   ![ toevoegen aan Slack ](../assets/add-to-slack.png)

   Als [!DNL Slack] is geïnstalleerd, wordt de toepassing geopend en wordt een bericht met het verzoek om toestemming weergegeven. Als de Slack niet geïnstalleerd is, moet u [ toestemming ](#slack-troubleshoot) verzoeken.

1. Klik op **[!UICONTROL Allow]**.

1. Schakel onder **[!UICONTROL Notifications]** [!DNL Slack] -meldingen in voor de gewenste producten en categorieën.

   ![ de berichten van de Slack ](../assets/slack.png)

   Updates voor meldingen worden automatisch opgeslagen.

### Machtiging aanvragen in [!DNL Slack] (problemen oplossen) {#slack-troubleshoot}

Als [!DNL Slack] niet is geïnstalleerd, wordt een _[!UICONTROL Request to install]_-bericht weergegeven wanneer de Slack wordt geopend nadat u op **[!UICONTROL Add to Slack]**hebt geklikt. Bijvoorbeeld:

![ Integratie van de Slack van het verzoek ](../assets/slack-workspace.png)

**om toestemmingen in Slack** te verzoeken

1. Selecteer in [!DNL Slack] de werkruimte in het menu **[!UICONTROL Workspace]** (rechterbovenhoek).

1. Klik op **[!UICONTROL Submit]** om goedkeuring van de toepassing aan te vragen voor het [!DNL Slack] -werkruimtebeheer.

1. U ontvangt een melding in [!DNL Slack] nadat de aanvraag is goedgekeurd.

1. Nadat u [!DNL Slack] goedkeuring ontvangt, terugkeer aan Experience Cloud **[!UICONTROL Notifications]** en volg de stappen aan [ intekenen aan Slack ](#slack-notifications) (hierboven beschreven).

### Wat u ziet in [!DNL Slack]

Nadat [!DNL Slack] met succes is geïntegreerd, geven de [!DNL Slack] -meldingen de volgende informatie weer:

* Het persoonlijke bericht zal van de toepassingsnaam _Adobe[!DNL Experience Cloud]_ worden ontvangen.
* Het bericht bevat het productlogo voor de specifieke toepassing, zoals Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager] enzovoort.
* Een koppeling om alle meldingen op het Experience Cloud weer te geven.
* Een koppeling voor het beheren van berichtgevingsvoorkeuren op Experience Cloud.

## Weergeven [!UICONTROL notifications] en aankondigingen in Experience Cloud {#view-notifications}

In de [!DNL Experience Cloud] kopbal, kunt u berichten bekijken waaraan u [ ](#notifications) intekende, evenals meningsaankondigingen.

1. Klik op het belpictogram in de koptekst. ![ Meldingen en Mededelingen ](../assets/bell-icon.png)

1. Klik op **[!UICONTROL Notifications]** of **[!UICONTROL Announcements]** .

   Op deze locatie ontvangt u belangrijke informatie over producten, uw samenwerking met andere gebruikers en andere relevante updates. De updates omvatten productversies, onderhoudsberichten, gedeelde punten, en goedkeuringsverzoeken.
