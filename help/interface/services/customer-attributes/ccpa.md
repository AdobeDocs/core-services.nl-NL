---
title: Customer Attributes Support for California Consumer Privacy Act
description: Meer informatie over Customer Attributes-ondersteuning voor California Consumer Privacy Act
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Customer Attributes support for California Consumer Privacy Act

Deze pagina beschrijft [!UICONTROL Customer Attributes]&quot;support for the California Consumer Privacy Act (CCPA).

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de CCPA.

De CCPA is de nieuwe privacywet van Californië, die 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te wissen en om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf, bepaalt u de persoonlijke gegevens die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, verleent Adobe Experience Cloud steun voor uw zaken om zijn verplichtingen uit hoofde van CCPA te vervullen die op het gebruik van de producten en de diensten van de Experience Cloud van toepassing zijn. Deze ondersteuning omvat het beheren van verzoeken om toegang tot en verwijdering van persoonlijke gegevens.

In dit document wordt beschreven hoe [!UICONTROL Customer Attributes] ondersteunt de CCPA-toegangsrechten en verwijderingsrechten voor gegevens van de betrokkenen via de API van Adobe Experience Platform Privacy Service en de gebruikersinterface van de Privacy Service.

Voor meer informatie over de diensten van de Privacy van de Adobe voor CCPA, zie [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Vereiste installatie voor het verzenden van aanvragen voor [!UICONTROL Customer Attributes]

Om verzoeken om tot gegevens toegang te hebben en te schrappen voor [!UICONTROL Customer Attributes], moet u:

1. Vermeld het volgende:

   * [Organisatie-ID](../../administration/organizations.md)
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Uw organisatie-id bestaat uit een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. U hebt de id van de organisatie nodig om aanvragen in te dienen bij de API voor privacy. Contact opnemen met de klantenservice van de Adobe op `gdprsupport@adobe.com` als u de id niet kunt vinden.

1. In [!UICONTROL Privacy Service], kunt u verzoeken om toegang en om verwijdering indienen bij Klantkenmerken en de status van bestaande aanvragen controleren.

## Vereiste veldwaarden in [!UICONTROL Customer Attributes] JSON-verzoeken

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*waarde van uw organisatie-id*>

&quot;gebruikers&quot;:

* &quot;key&quot;: &lt;*gewoonlijk de naam van de klant*>
* &quot;actie&quot;: **toegang** of **delete**
* &quot;gebruikers-id&#39;s&quot;:
   * &quot;namespace&quot;: &lt;*Alias-id van CRS-gegevensbron*>
   * &quot;type&quot;: **integrationCode**
   * &quot;value&quot;: &lt;*CRM-id*>
* &quot;include&quot;: **CRS** (dit is het Adobe product dat van toepassing is op het verzoek)
* &quot;verordening&quot;: **ccpa** (dit is de privacyverordening die van toepassing is op het verzoek)

## Voorbeeld van JSON-aanvraag

```json
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

```json
attributes:
{
"value": "<*value*>",
"key": "<*key*>",
"displayName": "<*displayName*>"
}
```
