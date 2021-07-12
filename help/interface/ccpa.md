---
title: 'Customer Attributes Support for California Consumer Privacy Act '
description: Meer informatie over Customer Attributes-ondersteuning voor California Consumer Privacy Act
feature: Klantkenmerken
topic: Beheer
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 5%

---

# Customer Attributes support for California Consumer Privacy Act

Op deze pagina wordt [!UICONTROL Customer Attributes']-ondersteuning voor de California Consumer Privacy Act (CCPA) beschreven.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de (CCPA).

De CCPA is de nieuwe privacywet van Californië, die 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te wissen en om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf, bepaalt u de persoonlijke gegevens die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, verleent Adobe Experience Cloud steun voor uw zaken om zijn verplichtingen uit hoofde van CCPA te vervullen die op het gebruik van de producten en de diensten van de Experience Cloud van toepassing zijn. Deze ondersteuning omvat het beheren van verzoeken om toegang tot en verwijdering van persoonlijke gegevens.

Dit document beschrijft hoe [!UICONTROL Customer Attributes] de gegevens CCPA van uw betrokkenen toegang en schrappingsrechten gebruikend Adobe Experience Platform Privacy Service API en Privacy Service UI steunt.

Voor meer informatie over de diensten van de Privacy van de Adobe voor CCPA, zie [het Centrum van de Privacy van de Adobe](https://www.adobe.com/privacy/ccpa.html).

## Vereiste installatie voor het verzenden van aanvragen voor [!UICONTROL Customer Attributes]

Als u verzoeken wilt indienen om gegevens voor [!UICONTROL Customer Attributes] te openen en te verwijderen, moet u:

1. Vermeld het volgende:

   * IMS-organisatie-id
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. Als uw marketingteam of interne beheerder van het Adobe-systeem de IMS Org-id van uw organisatie niet kent, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org-id nodig om aanvragen in te dienen bij de Privacy-API.

1. In [!UICONTROL Privacy Service], kunt u verzoeken van de Toegang en van de Schrapping aan de Attributen van de Klant voorleggen, en de status van bestaande verzoeken controleren.

## Vereiste veldwaarden in [!UICONTROL Customer Attributes] JSON-verzoeken

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;waarde&quot;: &lt;*uw IMS-waarde voor organisatie-id*>

&quot;gebruikers&quot;:

* &quot;key&quot;: &lt;*gewoonlijk de naam van de klant*>

* &quot;actie&quot;: hetzij **access** of **delete**

* &quot;gebruikers-id&#39;s&quot;:

   * &quot;namespace&quot;: &lt;*Alias-id van CRS-gegevensbron*>

   * &quot;type&quot;: **integrationCode**

   * &quot;waarde&quot;: &lt;*CRM-id*>

* &quot;include&quot;: **CRS** (dit is het product van Adobe dat op het verzoek van toepassing is)

* &quot;verordening&quot;: **ccpa** (dit is de privacyverordening die op het verzoek van toepassing is)

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
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
