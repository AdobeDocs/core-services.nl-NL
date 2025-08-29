---
description: Leer hoe te om het  [!DNL Customer Attributes]  schema in Adobe Experience Cloud te bevestigen.
solution: Experience Cloud
title: Hoe te om het  [!DNL Customer Attributes]  Schema te bevestigen
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: d2244e249c7af27bc1b4fc7bfe628bc25b37f4d4
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Het schema valideren

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort).

Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. De oorspronkelijke gegevens worden niet gewijzigd door het toewijzingsproces.

>[!NOTE]
>
>Wanneer u het schema bijwerkt nadat de validatie is uitgevoerd, worden de klantkenmerken verwijderd. Zie [ het schema bijwerken (schrapt ook attributen) ](t-crs-usecase.md).

**om het schema** te bevestigen

1. Klik in [!DNL Customer Attributes] op de kenmerkbron die u wilt bewerken.

1. Klik op **[!UICONTROL Edit Customer Attribute Source]** in het **[!UICONTROL File Upload]** .

1. Klik op de pagina [!UICONTROL File Upload and Schema Validation] op **[!UICONTROL Actions]** > **[!UICONTROL View/Edit Schema]** .

   ![ geef een schema ](assets/actions.png) uit

   Op de pagina [!UICONTROL Edit Schema] vertegenwoordigt elke rij van het schema een kolom van het geüploade CSV-bestand.

   ![ geef schemapagina in Experience Cloud uit ](assets/schema-edit.png)

**Acties**

* **[!UICONTROL Add Data:]** Nieuwe kenmerkgegevens uploaden naar deze gegevensbron.

* **[!UICONTROL View/Edit Schema:]** Wijs weergavenamen toe aan de kenmerkgegevens, zoals in de volgende stap wordt beschreven.

* **[!UICONTROL FTP Setup:]** creeer uw rekening van FTP aan [ uploadt uw gegevens via FTP ](t-upload-attributes-ftp.md) (facultatief).

* **[!UICONTROL ID Lookup:]** Voer een klant-id (CID) in van uw `.csv` om Experience Cloud-gegevens voor de id op te zoeken. Deze functie is handig voor het oplossen van problemen waarom kenmerkgegevens niet worden weergegeven voor een bezoeker:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Geeft weer als u de nieuwste Experience Cloud ID Service gebruikt. Als u zich op de MCID-service bevindt maar er hier geen id&#39;s worden vermeld, heeft Experience Cloud geen alias voor die CID ontvangen. Dit betekent dat de bezoeker zich niet heeft aangemeld of dat uw implementatie die id niet doorgeeft.

   * **[!UICONTROL CID (customer ID):]** De kenmerken die aan deze CID zijn gekoppeld. Als u een prop of eVar gebruikt om CID&#39;s (AVID) te uploaden en kenmerken worden weergegeven maar geen AVID, geeft dit aan dat de bezoeker zich niet bij uw site heeft aangemeld.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Hiermee wordt weergegeven als u een proxy of eVar gebruikt om CID&#39;s te uploaden. Als deze id&#39;s worden doorgegeven aan Experience Cloud, worden alle bezoekers-id&#39;s die zijn gekoppeld aan de ingevoerde CID hier weergegeven.
