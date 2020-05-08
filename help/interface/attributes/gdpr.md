---
title: Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening
description: Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening
translation-type: tm+mt
source-git-commit: 3a86aed0794c3e35cc028e5bfde5dafcb2285fc8
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening


>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de algemene verordening inzake gegevensbescherming.

De [algemene gegevensbeschermingsverordening](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html) (GDPR), die op 25 mei 2018 van kracht is, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens en vereenvoudigt het regelgevingskader voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud fungeert als gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe Customer Attributes de toegang tot en het verwijderen van GDPR-gegevens van de betrokkenen ondersteunt met behulp van de API en de gebruikersinterface van de privacyservice van het Adobe Experience Platform Privacy Service.

Raadpleeg [GDPR en Uw bedrijf](https://www.adobe.com/privacy/general-data-protection-regulation.html)voor meer informatie over wat GDPR voor uw bedrijf betekent.

## Vereiste installatie om verzoeken om klantkenmerken te verzenden

Om verzoeken om tot gegevens voor de Attributen van de Klant toegang te hebben en te schrappen, zult u moeten:

1. Vermeld het volgende:

* IMS Org ID
* Alias-id van CRS-gegevensbron waarop u wilt reageren
* CRM-id van het profiel waarop u wilt reageren

Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. Als uw marketingteam of interne Adobe-systeembeheerder de IMS Org-id van uw organisatie niet kent, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org-id nodig om aanvragen in te dienen bij de Privacy-API.

2. Gebruik de gebruikersinterface van de privacyservice om toegang te verzenden en verzoeken te verwijderen naar Customer Attributes en om de status van bestaande aanvragen te controleren.

## Vereiste veldwaarden in JSON-verzoeken wegens klantkenmerken

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;waarde&quot;: &lt;*uw IMS Org ID-waarde*>

&quot;gebruikers&quot;:

* &quot;key&quot;: &lt;*gewoonlijk de naam van de klant*>

* &quot;actie&quot;: of **toegang** of **schrapping**

* &quot;gebruikers-id&#39;s&quot;:

   * &quot;namespace&quot;: &lt;*Alias-id van CRS-gegevensbron*>

   * &quot;type&quot;: **integrationCode**

   * &quot;waarde&quot;: &lt;*CRM-id*>

* &quot;include&quot;: **CRS** (het Adobe-product dat van toepassing is op de aanvraag)

* &quot;verordening&quot;: **gdpr** ( de privacyverordening die op het verzoek van toepassing is )

## Voorbeeld van JSON-aanvraag

```
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "<IMS_ORG_ID>"
    }
  ],
  "users": [
    {
      "key": "<KEY>",
      "action": [
        "<access/delete>"
      ],
      "userIDs": [
        {
          "namespace": "<Alias ID of CRS Data Source>",
          "type": "integrationCode",
          "value": "<CRM ID>"
        }
      ]
    }
  ],
  "regulation": "<gdpr/ccpa/pdpa>",
  "include": [
    "CRS"
  ]
}
```

## Gegevensvelden die worden geretourneerd voor toegangsaanvragen

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
