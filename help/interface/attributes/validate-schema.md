---
description: Leer hoe u het klantkenmerkschema in Adobe Experience Cloud kunt valideren.
keywords: Klantkenmerken;Experience Cloud services
solution: Experience Cloud
title: 'Hoe te om het schema van de klantenattributen te bevestigen '
uuid: 163a4dbe-d60b-4089-8ff8-65f7461fbdf7
feature: Customer Attributes
topic: Administration
role: Administrator
level: Experienced
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Het schema valideren

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. Met dit toewijzingsproces worden de oorspronkelijke gegevens niet gewijzigd.

>[!NOTE]
>
>Wanneer u het schema bijwerkt nadat de validatie is uitgevoerd, worden de klantkenmerken verwijderd. Zie [Het schema bijwerken (schrapt ook attributen)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL View/Edit Schema]**

![](assets/view_edit_schema.png)

Op de [!UICONTROL Validate Schema] pagina, vertegenwoordigt elke rij van het schema een kolom van het geupload Csv- dossier.

![](assets/06_crs_usecase.png)

* **[!UICONTROL Add Data:]** Nieuwe kenmerkgegevens uploaden naar deze gegevensbron.

* **[!UICONTROL View/Edit Schema:]** Wijs weergavenamen toe aan de kenmerkgegevens, zoals in de volgende stap wordt beschreven.

* **[!UICONTROL FTP Setup:]** [Upload de gegevens via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

* **[!UICONTROL ID Lookup:]** Voer een Customer ID (CID) van je in  `.csv` om Experience Cloud-gegevens voor de id op te zoeken. Deze functie is handig voor het oplossen van problemen waarom kenmerkgegevens niet worden weergegeven voor een bezoeker:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Toont als u de recentste Dienst van identiteitskaart van Experience Cloud gebruikt. Als u zich op de dienst MCID bevindt maar geen IDs hier vermeld is, heeft de Experience Cloud geen alias voor die CID ontvangen. Dit betekent dat de bezoeker zich niet heeft aangemeld of dat uw implementatie die id niet doorgeeft.

   * **[!UICONTROL CID (Customer ID):]** De kenmerken die aan deze CID zijn gekoppeld. Als u een profiel of eVar gebruikt om CID&#39;s (AVID) te uploaden en u kenmerken ziet die worden weergegeven maar geen AVID, geeft dit aan dat de bezoeker zich niet heeft aangemeld bij uw site.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Hier wordt weergegeven of u CID&#39;s uploadt met een proxy of eVar. Als deze id&#39;s worden doorgegeven aan de Experience Cloud, worden hier alle bezoekers-id&#39;s weergegeven die zijn gekoppeld aan de ingevoerde CID.

U kunt gegevens ook uploaden via FTP nadat u een bron voor klantkenmerken en een FTP-account in de Experience Cloud hebt gemaakt. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten de .csv-indeling hebben, met een tweede .fin-bestand om aan te geven dat het uploaden is voltooid

De namen die u op koorden, gehelen, en aantallen toepast worden gebruikt om [!DNL Analytics] metriek tot stand te brengen. Zie [Rapport Klantkenmerken](https://docs.adobe.com/help/en/analytics/components/variables/dimensions-reports/reports-customer-attributes.html) in [!DNL Analytics] Help voor meer informatie.

* **[!UICONTROL Attribute:]** Kenmerkgegevens die uit het geüploade  `.csv` bestand worden gelezen.

* **[!UICONTROL Type:]** Het gegevenstype, zoals:

   * **Tekenreeks:** een reeks tekens.

   * **Geheel getal:** geheel getal

   * **Getallen:** kan uit maximaal twee decimalen bestaan.

* **[!UICONTROL Display Name:]** Een vriendelijke naam voor het kenmerk. U kunt bijvoorbeeld een kenmerk *leeftijd van klant* wijzigen in *Klant Since*.

* **[!UICONTROL Description:]** Een vriendelijke beschrijving van het kenmerk.
