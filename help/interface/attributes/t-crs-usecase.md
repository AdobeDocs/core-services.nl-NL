---
description: Creeer de bron van de klantenattributen en upload de gegevens.
keywords: Customer Attributes;core services
seo-description: Creeer de bron van de klantenattributen en upload de gegevens.
seo-title: Een bron voor klantkenmerken maken en het gegevensbestand uploaden
solution: Experience Cloud
title: Een bron voor klantkenmerken maken en het gegevensbestand uploaden
uuid: 53dca789-9a91-4385-839d-c9d1aa36b9be
translation-type: tm+mt
source-git-commit: af5201da6eac644e150783195bdbc8f93760c3f1
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---


# Een bron voor klantkenmerken maken en het gegevensbestand uploaden

Maak de bron van het klantkenmerk (CSV- en FIN-bestanden) en upload de gegevens. U kunt de gegevensbron activeren wanneer u klaar bent. Nadat de gegevensbron actief is, deel de attributengegevens aan Analytics en Doel.

## Workflow voor klantkenmerken {#concept_BF0AF88E9EF841219ED4D10754CD7154}

![](assets/crs.png)

1. [Een gegevensbestand maken](../attributes/t-crs-usecase.md#task_B5FB8C0649374C7A94C45DCF2878EA1A)
1. [De kenmerkbron maken en het gegevensbestand uploaden](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Het schema valideren](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Abonnementen configureren en kenmerkbron activeren](../attributes/t-crs-usecase.md#task_1ACA21198F0E46A897A320C244DFF6EA)

Nadat de gegevensbron actief is, kunt u:

* [Klantkenmerken gebruiken in Adobe Analytics](../attributes/t-crs-usecase.md#task_7EB0680540CE4B65911B2C779210915D)
* [Klantkenmerken gebruiken in Adobe Target](../attributes/t-crs-usecase.md#task_FC5F9D9059114027B62DB9B1C7D9E257)

>[!IMPORTANT]
>
>Om toegang te krijgen tot deze functie, moeten gebruikers worden toegewezen aan het productprofiel Klantkenmerken (Klantkenmerken - Standaardtoegang). Ga naar **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. Als *Klantkenmerken* als een van de [!UICONTROL Product Profiles]kenmerken worden weergegeven, kunt u beginnen. Gebruikers die aan de groep Klantkenmerken zijn toegevoegd, zien het [!UICONTROL Customer Attributes] menu links in de interface Experience Cloud.
>
>Om de eigenschap van de Attributen van de Klant te gebruiken, moeten de gebruikers tot oplossing-vlakke groepen (Analytics of [!DNL Target]) ook behoren.

See [Manage Experience Cloud users and products](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9).

## Een gegevensbestand maken {#task_B5FB8C0649374C7A94C45DCF2878EA1A}

Dit gegeven is gegevens van ondernemingsklanten van uw CRM. De gegevens kunnen abonneegegevens voor producten bevatten, waaronder id&#39;s van leden, producten met de naam, de meest gestarte producten enzovoort.

1. Maak een `.csv`.

   >[!NOTE]
   >
   >Later in dit proces, zult u slepen-en-dalings het `.csv` om het dossier te uploaden. Als u echter [uploadt via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B), hebt u ook een `.fin` bestand nodig met dezelfde naam als de `.csv`.

   Voorbeeld bedrijfsklantenbestand:

   ![](assets/01_crs_usecase.png)

1. Voordat u verdergaat, bekijkt u eerst de belangrijke informatie in [Gegevensbestandsvereisten](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19)voordat u het bestand uploadt.
1. [Maak een bron voor klantkenmerken en upload de gegevens](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78), zoals hieronder beschreven.

## De kenmerkbron maken en het gegevensbestand uploaden {#task_09DAC0F2B76141E491721C1E679AABC8}

Voer deze stappen op de Create Nieuwe Bron van Attributen van de Klant in de Cloud van de Ervaring uit.

>[!IMPORTANT]
>
>Wanneer het creëren van, het wijzigen van, of het schrappen van de bronnen van de klantenattributen, is er een vertraging van maximaal één uur alvorens IDs begint synchroniserend met de nieuwe gegevensbron. U moet administratieve rechten in de Manager van de Publiek hebben om de bronnen van de klantenattributen tot stand te brengen of te wijzigen. Neem contact op met de klantenservice of het advies van de Audience Manager om beheerrechten te verkrijgen.

1. Klik in het [!DNL Experience Cloud]deelvenster op het ![](assets/menu-icon.png) pictogram Menu.
1. Klik onder **[!DNL Experience Platform]** op **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**.

   Op de [!UICONTROL Customer Attributes] pagina kunt u bestaande bronnen met kenmerkgegevens beheren en bewerken.

   ![Stap resultaat](assets/03_crs_usecase.png)
1. Klik op **[!UICONTROL New]**.

   ![Stap resultaat](assets/04_crs_usecase.png)
1. Configureer op de [!UICONTROL Edit Customer Attribute Source] pagina de volgende velden:

   * **[!UICONTROL Name:]** Een vriendelijke naam voor de bron van het gegevenskenmerk. Kenmerknamen mogen bijvoorbeeld geen spaties bevatten. [!DNL Adobe Target] Wanneer een kenmerk met een spatie wordt doorgegeven, wordt dit [!DNL Target] genegeerd. Andere tekens worden niet ondersteund: `< , >, ', "`.

   * **[!UICONTROL Description:]** (Optioneel) Een beschrijving van de bron van het gegevenskenmerk.

   * **[!UICONTROL Alias ID:]** Vertegenwoordigt een bron van de gegevens van de klanteneigenschap, zoals een specifiek systeem van CRM. Een unieke id die wordt gebruikt in de broncode van het kenmerk Klant. De id moet uniek zijn, in kleine letters en zonder spaties. De waarde die wordt ingevoerd in het veld Alias-id voor een bron van klantkenmerken in de gebruikersinterface van de Experience Cloud moet overeenkomen met de waarden die worden doorgegeven vanuit de implementatie (via dynamisch tagbeheer of JavaScript van de Mobile SDK.)

      De alias-id komt overeen met bepaalde gebieden waar u extra waarden voor de klant-id instelt. Bijvoorbeeld:

      * **Dynamisch tagbeheer:** De Alias-id komt overeen met de waarde voor *Integratiecode* onder [!UICONTROL Customer Settings], in het [Experience Cloud ID-hulpprogramma](https://docs.adobe.com/content/help/en/dtm/using/tools/macid.html) .

      * **Bezoeker-API:** De Alias-id komt overeen met de extra [klant-id&#39;s](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) die u aan elke bezoeker kunt koppelen.

         Bijvoorbeeld *&quot;crm_id&quot;* in:

         ```
         "crm_id":"67312378756723456"
         ```

      * **iOS:** De alias-id komt overeen met *&quot;idType&quot;* in [bezoekerSyncIdentifiers:IDs](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html).

         Bijvoorbeeld:

         `[ADBMobile visitorSyncIdentifiers:@{@<`**`"idType"`**`:@"idValue"}];`

      * **Android:** De alias-id komt overeen met *&quot;idType&quot;* in [syncIdentifiers](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html).

         Bijvoorbeeld:

         `identifiers.put(`**`"idType"`**`, "idValue");`

         Zie Meerdere gegevensbronnen [](../attributes/crs-data-file.md#section_76DEB6001C614F4DB8BCC3E5D05088CB) benutten voor aanvullende informatie over gegevensverwerking met betrekking tot het veld Alias-id en de id&#39;s van de klant.
   * **[!UICONTROL File Upload:]** U kunt het `.csv` gegevensbestand slepen en neerzetten, of de gegevens uploaden via FTP. (Voor het gebruik van FTP is ook een `.fin` bestand vereist.) Zie De gegevens [uploaden via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

      >[!IMPORTANT]
      >
      >Er zijn specifieke gegevensbestandsvereisten. Zie [Gegevensbestandsvereisten](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) voor meer informatie.


      Nadat u het bestand hebt geüpload, worden tabelgegevens onder de [!UICONTROL File Upload] kop op deze pagina weergegeven. U kunt het schema valideren, abonnementen configureren of de FTP instellen.

      **Afbeelding voor uploaden bestand**

      ![](assets/file_upload_attributes.png)

   * **[!UICONTROL Unique Customer ID:]** Hiermee geeft u weer hoeveel unieke id&#39;s u naar deze kenmerkbron hebt geüpload.

   * **[!UICONTROL Customer-Provided IDs Aliased to Experience Cloud Visitor IDs:]** Hiermee geeft u weer hoeveel id&#39;s zijn aliased voor Experience Cloud Visitor-id&#39;s.

   * **[!UICONTROL Customer-Provided IDs with High Alias Counts:]** Geeft het aantal door de klant geleverde id&#39;s weer met 500 of meer Aliased Experience Cloud Visitor-id&#39;s. Deze door de klant opgegeven id&#39;s vertegenwoordigen hoogstwaarschijnlijk geen personen, maar een soort gedeelde aanmelding. Het systeem verdeelt de attributen verbonden aan deze IDs aan 500 meest recente aliased Ervaring Cloud Bezoeker IDs, tot het aliasaantal 10.000 bereikt. Op dat moment maakt het systeem de door de klant opgegeven id ongeldig en worden de bijbehorende kenmerken niet meer gedistribueerd.



## Het schema valideren {#task_404AAC411B0D4E129AB3AC8B7BE85859}

Met het validatieproces kunt u weergavenamen en beschrijvingen toewijzen aan geüploade kenmerken (tekenreeksen, gehele getallen, getallen, enzovoort). U kunt kenmerken ook verwijderen door het schema bij te werken.

Zie Het schema [](../attributes/validate-schema.md#concept_B3A01A15D04E4F998118E09B3A9B5043)valideren.

Zie [(Optioneel) Het schema bijwerken (kenmerken verwijderen)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C)om kenmerken te verwijderen.

## (Optioneel) Werk het schema bij (verwijder kenmerken) {#task_6568898BB7C44A42ABFB86532B89063C}

Hoe te om attributen te schrappen en attributen in het schema te vervangen.

1. Verwijder op de [!UICONTROL Edit Customer Attribute Source] pagina het **[!UICONTROL Target]** of het **[!UICONTROL Analytics]** abonnement (onder [!UICONTROL Configure Subscriptions]).
1. [Upload een nieuw gegevensbestand met bijgewerkte gebieden](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8).

## Abonnementen configureren en kenmerkbron activeren {#task_1ACA21198F0E46A897A320C244DFF6EA}

Als u een abonnement configureert, wordt de gegevensstroom ingesteld tussen de Experience Cloud en de oplossingen. Door de kenmerkbron te activeren, kunnen de gegevens naar ingetekende oplossingen stromen. De klantrecords die u hebt geüpload, komen overeen met binnenkomende id-signalen van uw website of toepassing.

Zie Abonnementen [configureren](../attributes/subscription.md#concept_ECA3C44FA6D540C89CC04BA3C49E63BF).

**Een kenmerkbron activeren**

Zoek op de pagina [!UICONTROL Create New [or Edit] Customer Attribute Source] de [!UICONTROL Activate] kop en klik op **[!UICONTROL Active]**.

![Stap resultaat](assets/activate_attribute_source.png)

## Klantkenmerken gebruiken in Adobe Analytics {#task_7EB0680540CE4B65911B2C779210915D}

Met de gegevens die nu beschikbaar zijn in oplossingen zoals
<keyword>
Adobe Analytics
</keyword>kunt u de gegevens rapporteren, analyseren en de juiste actie ondernemen in uw marketingcampagnes.

In het volgende voorbeeld wordt een [!DNL Analytics] segment weergegeven op basis van de geüploade kenmerken. Dit segment toont [!DNL Photoshop Lightroom] abonnees van wie het meest-gelanceerde product Photoshop is.

![](assets/08_crs_usecase.png)

Wanneer u een segment publiceert naar de Experience Cloud, wordt het beschikbaar in Experience Cloud Audiences en Audience Manager.

Zie Rapport [Klantkenmerken](https://docs.adobe.com/help/en/analytics/components/variables/dimensions-reports/reports-customer-attributes.html) in Analytics Help voor meer informatie.

## Klantkenmerken gebruiken in Adobe Target {#task_FC5F9D9059114027B62DB9B1C7D9E257}

In [!DNL Target], kunt u een klantenattribuut van de [!UICONTROL Visitor Profile] sectie selecteren wanneer het creëren van een publiek. Alle Klantkenmerken hebben het voorvoegsel [!DNL crs.] in de lijst. U kunt deze kenmerken desgewenst combineren met andere gegevenskenmerken om een publiek te maken.

![](assets/crs-add-attribute-target.png)

Zie [Een nieuw publiek](https://docs.adobe.com/content/help/en/target/using/audiences/create-audiences/audiences.html) maken in de [!DNL Target] Help.
