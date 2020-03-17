---
description: Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. Met dit toewijzingsproces worden de oorspronkelijke gegevens niet gewijzigd.
keywords: customer attributes;core services
seo-description: Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. Met dit toewijzingsproces worden de oorspronkelijke gegevens niet gewijzigd.
seo-title: Het schema valideren
solution: Experience Cloud
title: Het schema valideren
uuid: 163a4dbe-d60b-4089-8ff8-65f7461fbdf7
translation-type: tm+mt
source-git-commit: 73cb227d2b44024706ce24a9ae6aa06c57a8ce85

---


# Het schema valideren

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. Met dit toewijzingsproces worden de oorspronkelijke gegevens niet gewijzigd.

>[!NOTE]
>
>Wanneer u het schema bijwerkt nadat de validatie is uitgevoerd, worden de klantkenmerken verwijderd. Zie Het schema [bijwerken (kenmerken worden ook verwijderd)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL View/Edit Schema]**

![](assets/view_edit_schema.png)

Op de [!UICONTROL Validate Schema] pagina vertegenwoordigt elke rij van het schema een kolom van het geüploade CSV-bestand.

![](assets/06_crs_usecase.png)

* **[!UICONTROL Add Data:]** Nieuwe kenmerkgegevens uploaden naar deze gegevensbron.

* **[!UICONTROL View/Edit Schema:]** Wijs weergavenamen toe aan de kenmerkgegevens, zoals in de volgende stap wordt beschreven.

* **[!UICONTROL FTP Setup:]** De gegevens [uploaden via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

* **[!UICONTROL ID Lookup:]** Voer een klant-id (CID) van uw computer in `.csv` om de gegevens van Experience Cloud voor de id op te zoeken. Deze functie is handig voor het oplossen van problemen waarom kenmerkgegevens niet worden weergegeven voor een bezoeker:

   * **[!UICONTROL MCID (Experience Cloud ID):]** Geeft weer als u de nieuwste Experience Cloud ID Service gebruikt. Als u op de MCID-service werkt maar hier geen id&#39;s worden vermeld, heeft de Experience Cloud geen alias voor die CID ontvangen. Dit betekent dat de bezoeker zich niet heeft aangemeld of dat uw implementatie die id niet doorgeeft.

   * **[!UICONTROL CID (Customer ID):]** De kenmerken die aan deze CID zijn gekoppeld. Als u een prop of eVar gebruikt om CID&#39;s (AVID) te uploaden, en u weergegeven kenmerken ziet maar geen AVID, geeft dit aan dat de bezoeker zich niet bij uw site heeft aangemeld.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Hier wordt weergegeven of u CID&#39;s uploadt met een proxy of eVar. Als deze id&#39;s worden doorgegeven aan de Experience Cloud, worden alle bezoekers-id&#39;s die zijn gekoppeld aan de ingevoerde CID hier weergegeven.

U kunt gegevens ook uploaden via FTP nadat u een bron voor klantkenmerken en een FTP-account hebt gemaakt in de Experience Cloud. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten de .csv-indeling hebben, met een tweede .fin-bestand om aan te geven dat het uploaden is voltooid

De namen die u toepast op tekenreeksen, gehele getallen en getallen worden gebruikt om [!DNL Analytics] metriek te maken. Zie Rapport [Klantkenmerken](https://docs.adobe.com/help/en/analytics/components/variables/dimensions-reports/reports-customer-attributes.html) in [!DNL Analytics] Help voor meer informatie.

* **[!UICONTROL Attribute:]** Kenmerkgegevens die uit het geüploade `.csv` bestand worden gelezen.

* **[!UICONTROL Type:]** Het gegevenstype, zoals:

   * **Tekenreeks:** Een reeks tekens.

   * **Geheel getal:** Hele getallen.

   * **Getallen:** Kan uit maximaal twee decimalen bestaan.

* **[!UICONTROL Display Name:]** Een vriendelijke naam voor het kenmerk. Bijvoorbeeld, zou u een *klantenleeftijd* van attributen aan *Klant kunnen veranderen Sopend*.

* **[!UICONTROL Description:]** Een vriendelijke beschrijving van het kenmerk.
