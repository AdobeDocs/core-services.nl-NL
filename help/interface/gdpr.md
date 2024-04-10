---
title: "[!DNL Customer Attributes] Steun voor de algemene verordening inzake gegevensbescherming"
description: Meer informatie over Customer Attributes Support for General Data Protection Regulation
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# [!DNL Customer Attributes] steun voor de algemene verordening inzake gegevensbescherming

Deze pagina beschrijft hoe [!DNL Customer Attributes] ondersteunt algemene gegevensbeschermingsverordening (GDPR).

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies of is bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de GDPR.

De [Algemene verordening inzake gegevensbescherming](https://business.adobe.com/privacy/general-data-protection-regulation.html), een wet die van kracht is op 25 mei 2018, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens. Het vereenvoudigt ook de regelgeving voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud treedt op als een gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe [!DNL Customer Attributes] ondersteunt de toegangsrechten voor GDPR-gegevens en verwijderingsrechten van de betrokkenen via de API van Adobe Experience Platform Privacy Service en de gebruikersinterface van de Privacy Service.

Voor meer informatie over wat GDPR voor uw zaken betekent, zie [GDPR en uw bedrijf](https://business.adobe.com/privacy/general-data-protection-regulation.html).

## Vereiste installatie voor het verzenden van aanvragen voor [!DNL Customer Attributes]

Om verzoeken om tot gegevens toegang te hebben en te schrappen voor [!DNL Customer Attributes], moet u:

1. Vermeld het volgende:

   * [Organisatie-ID](#organizations.md)
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Uw [organisatie-id](#organizations.md) is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. U hebt de id van de organisatie nodig om aanvragen in te dienen bij de API voor privacy. Contact opnemen met de klantenservice van de Adobe op `gdprsupport@adobe.com` als u de id niet kunt vinden.

1. In [!UICONTROL Privacy Service], kunt u verzoeken om toegang en om verwijdering verzenden naar [!DNL Customer Attributes]en controleert u de status van bestaande verzoeken.

## Vereiste veldwaarden in [!DNL Customer Attributes] JSON-verzoeken

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*uw IMS Org ID-waarde*>

&quot;gebruikers&quot;:

* &quot;key&quot;: &lt;*gewoonlijk de naam van de klant*>

* &quot;actie&quot;: **toegang** of **delete**

* &quot;gebruikers-id&#39;s&quot;:

   * &quot;namespace&quot;: &lt;*Alias-id van CRS-gegevensbron*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM-id*>

* &quot;include&quot;: **CRS** (dit is het Adobe product dat van toepassing is op het verzoek)

* &quot;verordening&quot;: **gdpr** (dit is de privacyverordening die van toepassing is op het verzoek)

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

## Gegevensvelden die worden geretourneerd voor toegangsverzoeken

```
attributes:
{
"value":<*value*>,
"key":<*key*>,
"displayName":<*displayName*>
}
```
