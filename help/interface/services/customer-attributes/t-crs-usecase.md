---
description: Maak een kenmerkbron voor klanten en upload deze naar de Adobe Experience Cloud.
solution: Experience Cloud
title: Een kenmerkbron voor de klant maken en het gegevensbestand uploaden
uuid: 53dca789-9a91-4385-839d-c9d1aa36b9be
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 21ed7c35-aac9-46f1-a50c-84e7c075209c
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 1%

---

# Een bron voor klantkenmerken maken en het gegevensbestand uploaden

Maak de bron van klantkenmerken (CSV- en FIN-bestanden) en upload de gegevens. U kunt de gegevensbron activeren wanneer u klaar bent. Nadat de gegevensbron actief is, deel de attributengegevens aan Analytics en Doel.

## Workflow voor klantkenmerken {#concept_BF0AF88E9EF841219ED4D10754CD7154}

![Workflow voor klantkenmerken](assets/crs.png)

>[!IMPORTANT]
>
>Om toegang te krijgen tot deze functie, moeten gebruikers worden toegewezen aan het productprofiel Klantkenmerken (Klantkenmerken - Standaardtoegang). Ga naar **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. Indien *Klantkenmerken* wordt weergegeven als een van de [!UICONTROL product profiles], bent u klaar om te beginnen. De gebruikers die aan de groep van Attributen van de Klant worden toegevoegd zien [!UICONTROL Customer Attributes] aan de linkerkant van de interface Experience Cloud.
>
>Om de eigenschap van Attributen van de Klant te gebruiken, moeten de gebruikers tot toepassing-vlakke groepen (Analytics of [!DNL Target]).

## Een gegevensbestand maken {#task_B5FB8C0649374C7A94C45DCF2878EA1A}

Dit gegeven is gegevens van ondernemingsklanten van uw CRM. De gegevens kunnen abonneegegevens voor producten bevatten, waaronder id&#39;s van leden, producten met de naam, de meest gestarte producten enzovoort.

1. Een `.csv`.

   >[!NOTE]
   >
   >Later in dit proces kunt u de `.csv` het bestand uploaden. Als u echter [uploaden via FTP](t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B), hebt u ook `.fin` bestand met dezelfde naam als het `.csv`.

   Voorbeeld bedrijfsklantenbestand:

   ![Voorbeeld van een klantgegevensbestand voor ondernemingen](assets/01_crs_usecase.png)

1. Lees voordat u verdergaat de belangrijke informatie in [Gegevensbestandsvereisten](crs-data-file.md), voordat u het bestand uploadt.
1. [Een bron voor klantkenmerken maken en de gegevens uploaden](t-crs-usecase.md), zoals hieronder beschreven.

## De kenmerkbron maken en het gegevensbestand uploaden {#task_09DAC0F2B76141E491721C1E679AABC8}

Voer deze stappen op de Create Nieuwe Bron van Attributen van de Klant in Experience Cloud uit.

>[!IMPORTANT]
>
>Wanneer het creëren van, het wijzigen van, of het schrappen van de bronnen van de Attributen van de Klant, is er een vertraging van maximaal één uur alvorens IDs begint synchroniserend met de nieuwe gegevensbron. U moet beheerdersrechten in Audience Manager hebben om bronnen voor klantkenmerken te maken of te wijzigen. Neem contact op met de klantenservice of de Audience Manager voor advies om beheerrechten te verkrijgen.

1. In de [!DNL Experience Cloud], selecteert u het menu  ![menu](assets/menu-icon.png) pictogram.
1. Onder **[!DNL Experience Platform]**, selecteert u **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**.

   De [!UICONTROL Customer Attributes] op deze pagina kunt u bestaande bronnen met kenmerkgegevens beheren en bewerken.

   ![Stap Resultaat](assets/03_crs_usecase.png)

1. Selecteer **[!UICONTROL New]**.

   ![Stap Resultaat](assets/04_crs_usecase.png)

1. Op de [!UICONTROL Edit Customer Attribute Source] pagina, configureert u de volgende velden:

   * **[!UICONTROL Name:]** Een vriendelijke naam voor de bron van het gegevenskenmerk. Voor [!DNL Adobe Target], attribuutnamen mogen geen spaties bevatten. Als een kenmerk met een spatie wordt doorgegeven, [!DNL Target] negeert het. Andere tekens worden niet ondersteund: `< , >, ', "`.

   * **[!UICONTROL Description:]** (Optioneel) Een beschrijving van de bron van het gegevenskenmerk.

   * **[!UICONTROL Alias ID:]** Vertegenwoordigt een bron van de gegevens van de Attributen van de Klant, zoals een specifiek systeem van CRM. [!UICONTROL Alias ID] is een unieke id die wordt gebruikt in de broncode van uw kenmerk van de klant. De id moet uniek zijn, in kleine letters en zonder spaties. De waarde die wordt ingevoerd in het dialoogvenster [!UICONTROL Alias ID] voor een bron van de Attributen van de Klant in Experience Cloud zou de waarden moeten aanpassen die binnen van de implementatie (of via de Inzameling van de Gegevens van het Platform of JavaScript van Mobiele SDK worden overgegaan.)

     De alias-id komt overeen met bepaalde gebieden waar u extra waarden voor de klant-id instelt. Bijvoorbeeld:

      * **Dynamisch tagbeheer:** De alias-id komt overeen met de *Integratiecode* waarde onder [!UICONTROL Customer Settings]in de [Experience Cloud-id-service](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=nl) gebruiken.

      * **Bezoeker-API:** De alias-id komt overeen met de aanvullende [Klant-id&#39;s](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) die u aan elke bezoeker kunt koppelen.

        Bijvoorbeeld: *&quot;crm_id&quot;* in:

        ```
        "crm_id":"67312378756723456"
        ```

      * **iOS:** De alias-id komt overeen met *&quot;idType&quot;* in [bezoekerSyncIdentifiers:id&#39;s](https://experienceleague.adobe.com/docs/mobile-services/ios/overview.html).

        Bijvoorbeeld:

        `[ADBMobile visitorSyncIdentifiers:@{@<`**`"idType"`**`:@"idValue"}];`

      * **Android™:** De alias-id komt overeen met *&quot;idType&quot;* in [syncIdentifiers](https://experienceleague.adobe.com/docs/mobile-services/android/overview.html).

        Bijvoorbeeld:

        `identifiers.put(`**`"idType"`**`, "idValue");`

        Zie [Meerdere gegevensbronnen gebruiken](crs-data-file.md#section_76DEB6001C614F4DB8BCC3E5D05088CB) voor aanvullende informatie over gegevensverwerking met betrekking tot het veld Alias-id en de id&#39;s van de klant.

   * **[!UICONTROL File Upload:]** U kunt de `.csv` of uploadt u de gegevens via FTP. (Voor het gebruik van FTP is ook een `.fin` bestand.) Zie [De gegevens uploaden via FTP](t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

     >[!IMPORTANT]
     >
     >Er zijn specifieke gegevensbestandsvereisten. Zie [Gegevensbestandsvereisten](crs-data-file.md) voor meer informatie .


     Nadat u het bestand hebt geüpload, worden tabelgegevens weergegeven onder de [!UICONTROL File Upload] op deze pagina. U kunt het schema valideren, abonnementen configureren of de FTP instellen.

     **Afbeelding voor uploaden bestand**

     ![attributes](assets/file_upload_attributes.png)

   * **[!UICONTROL Unique Customer ID:]** Geeft aan hoeveel unieke id&#39;s u naar deze kenmerkbron hebt geüpload.

   * **[!UICONTROL Customer-Provided IDs Aliased to Experience Cloud Visitor IDs:]** Hiermee geeft u weer hoeveel id&#39;s zijn aliased aan Experience Cloud Visitor-id&#39;s.

   * **[!UICONTROL Customer-Provided IDs with High Alias Counts:]** Geeft het aantal door de klant opgegeven id&#39;s weer met 500 of meer aliased Experience Cloud Visitor-id&#39;s. Deze door de klant opgegeven id&#39;s vertegenwoordigen hoogstwaarschijnlijk geen personen, maar een soort gedeelde aanmelding. Het systeem verdeelt de attributen verbonden aan deze IDs aan 500 meest recente aliased Experience Cloud Bezoeker IDs, tot de aliastelling 10.000 bereikt. Vervolgens maakt het systeem de door de klant opgegeven id ongeldig en worden de bijbehorende kenmerken niet meer gedistribueerd.

## Het schema valideren {#task_404AAC411B0D4E129AB3AC8B7BE85859}

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). U kunt kenmerken ook verwijderen door het schema bij te werken.

Zie [Het schema valideren](validate-schema.md).

Zie voor informatie over het verwijderen van kenmerken [(Optioneel) Werk het schema bij (verwijder kenmerken)](t-crs-usecase.md).

## (Optioneel) Werk het schema bij (verwijder kenmerken) {#task_6568898BB7C44A42ABFB86532B89063C}

Hoe te om attributen te schrappen en attributen in het schema te vervangen.

1. Op de [!UICONTROL Edit Customer Attribute Source] pagina, verwijder de **[!UICONTROL Target]** of **[!UICONTROL Analytics]** abonnement (onder [!UICONTROL Configure Subscriptions]).
1. [Een nieuw gegevensbestand met bijgewerkte velden uploaden](t-crs-usecase.md).

## Abonnementen configureren en kenmerkbron activeren {#task_1ACA21198F0E46A897A320C244DFF6EA}

Als u een abonnement configureert, wordt de gegevensstroom tussen Experience Cloud en toepassingen ingesteld. Door de kenmerkbron te activeren, kunnen de gegevens naar geabonneerde toepassingen stromen. De klantrecords die u hebt geüpload, komen overeen met binnenkomende id-signalen van uw website of toepassing.

Zie [Abonnementen configureren](subscription.md).

**Een kenmerkbron activeren**

Op de [!UICONTROL Create New or Edit Customer Attribute Source] pagina, zoek de [!UICONTROL Activate] kop selecteert u vervolgens **[!UICONTROL Active]**.

![Stap Resultaat](assets/activate_attribute_source.png)

## Klantkenmerken gebruiken in Adobe Analytics {#task_7EB0680540CE4B65911B2C779210915D}

Met de gegevens die nu beschikbaar zijn in toepassingen zoals Adobe Analytics, kunt u de gegevens rapporteren, analyseren en de juiste actie ondernemen in uw marketingcampagnes.

In het volgende voorbeeld wordt een [!DNL Analytics] op basis van de geüploade kenmerken. Dit segment toont [!DNL Photoshop Lightroom] abonnees van wie het meest gelanceerde product Photoshop is.

![Segment Analytics op basis van de geüploade kenmerken](assets/08_crs_usecase.png)

Wanneer u een segment aan Experience Cloud publiceert, wordt het beschikbaar in het Publiek van het Experience Cloud en Audience Manager.

## Klantkenmerken gebruiken in Adobe Target {#task_FC5F9D9059114027B62DB9B1C7D9E257}

In [!DNL Target], kunt u een kenmerk van de klant selecteren in het menu [!UICONTROL Visitor Profile] bij het maken van een publiek. Alle klantkenmerken hebben het voorvoegsel `crs.` in de lijst. U kunt deze kenmerken desgewenst combineren met andere gegevenskenmerken om een publiek te maken.

![Klantkenmerken gebruiken in Adobe Target](assets/crs-add-attribute-target.png)

Zie [Een nieuw publiek maken](https://experienceleague.adobe.com/docs/target/using/audiences/create-audiences/audiences.html) in [!DNL Target] help.
