---
description: Leer hoe u het klantkenmerkschema in Adobe Experience Cloud kunt valideren.
solution: Experience Cloud
title: Hoe te om het Schema van Attributen van de Klant te bevestigen
uuid: 163a4dbe-d60b-4089-8ff8-65f7461fbdf7
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Het schema valideren

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). Op basis van deze instellingen wordt een schema gemaakt. Het schema wordt gebruikt om alle toekomstige gegevens te bevestigen die aan deze gegevensbron worden geupload. De oorspronkelijke gegevens worden niet gewijzigd door het toewijzingsproces.

>[!NOTE]
>
>Wanneer u het schema bijwerkt nadat de validatie is uitgevoerd, worden de klantkenmerken verwijderd. Zie [ het schema bijwerken (schrapt ook attributen) ](t-crs-usecase.md).

**[!UICONTROL Customer Attribute Source]** > **[!UICONTROL Create New Customer Attribute Source]** > **[!UICONTROL View/Edit Schema]**

![ geef een schema ](assets/view_edit_schema.png) uit

Op de pagina [!UICONTROL Validate Schema] vertegenwoordigt elke rij van het schema een kolom van het geüploade CSV-bestand.

![ bevestigt schemapagina in Experience Cloud ](assets/06_crs_usecase.png)

* **[!UICONTROL Add Data:]** Nieuwe kenmerkgegevens uploaden naar deze gegevensbron.

* **[!UICONTROL View/Edit Schema:]** Wijs weergavenamen toe aan de kenmerkgegevens, zoals in de volgende stap wordt beschreven.

* **[!UICONTROL FTP Setup:]** [ uploadt de gegevens via FTP ](t-upload-attributes-ftp.md).

* **[!UICONTROL ID Lookup:]** Voer een CID (Customer ID) van uw `.csv` in om de gegevens van het Experience Cloud voor de id op te zoeken. Deze functie is handig voor het oplossen van problemen waarom kenmerkgegevens niet worden weergegeven voor een bezoeker:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Geeft weer als u de nieuwste Experience Cloud-id-service gebruikt. Als u zich op de dienst MCID bevindt maar geen IDs hier vermeld is, heeft het Experience Cloud geen alias voor die CID ontvangen. Dit betekent dat de bezoeker zich niet heeft aangemeld of dat uw implementatie die id niet doorgeeft.

   * **[!UICONTROL CID (Customer ID):]** De kenmerken die aan deze CID zijn gekoppeld. Als u een profiel of eVar gebruikt om CID&#39;s (AVID) te uploaden en u kenmerken ziet die worden weergegeven maar geen AVID, geeft dit aan dat de bezoeker zich niet heeft aangemeld bij uw site.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Hiermee wordt weergegeven als u CID&#39;s uploadt met een proxy of eVar. Als deze id&#39;s worden doorgegeven aan het Experience Cloud, worden hier alle bezoekers-id&#39;s weergegeven die zijn gekoppeld aan de ingevoerde CID.

U kunt gegevens ook uploaden via FTP nadat u een bron voor klantkenmerken en een FTP-account in Experience Cloud hebt gemaakt. U maakt één FTP-account per kenmerkbron. De geüploade bestanden worden opgeslagen in de hoofdmap van dat account. De gegevens moeten de `.csv` -indeling hebben, met een tweede `.fin` -bestand om aan te geven dat het uploaden is voltooid.

De namen die u toepast op tekenreeksen, gehele getallen en getallen worden gebruikt om [!DNL Analytics] -metriek te maken.

* **[!UICONTROL Attribute:]** Kenmerkgegevens die uit het geüploade `.csv` -bestand worden gelezen.

* **[!UICONTROL Type:]** Het gegevenstype, zoals:

   * **Koord:** een opeenvolging van karakters.

   * **Gehele aantallen:** Gehele aantallen.

   * **Aantallen:** kan tot twee decimalen hebben.

* **[!UICONTROL Display Name:]** Een vriendelijke naam voor het kenmerk. Bijvoorbeeld, kunt u een attribuut *klantenleeftijd* aan *Klant veranderen aangezien*.

* **[!UICONTROL Description:]** Een vriendelijke beschrijving van het kenmerk.
