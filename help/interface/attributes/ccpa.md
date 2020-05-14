---
title: Customer Attributes Support for California Consumer Privacy Act
description: Customer Attributes Support for California Consumer Privacy Act
translation-type: tm+mt
source-git-commit: 4223f9260865756842ad43b99d2509908f4d6572
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---


# Customer Attributes support for California Consumer Privacy Act

Op deze pagina wordt de [!UICONTROL Customer Attributes'] ondersteuning voor de California Consumer Privacy Act (CCPA) beschreven.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de (CCPA).

De CCPA is de nieuwe privacywet van Californië, die 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te verwijderen, alsmede het recht om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

Als prepressbureau biedt Adobe Experience Cloud ondersteuning voor uw bedrijf om te voldoen aan de verplichtingen in het kader van de CCPA die van toepassing zijn op het gebruik van producten en services van Experience Cloud, waaronder het beheren van verzoeken om toegang tot en verwijdering van persoonlijke gegevens.

In dit document wordt beschreven hoe de toegangsrechten en verwijderingsrechten voor CCPA-gegevens van de betrokkenen worden [!UICONTROL Customer Attributes] ondersteund met de API en gebruikersinterface van de Adobe Experience Platform Privacy Service.

Ga naar het [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html)voor meer informatie over de Adobe-privacyservices voor CCPA.

## Vereiste installatie voor het verzenden van aanvragen voor [!UICONTROL Customer Attributes]

Als u verzoeken wilt indienen om gegevens te openen en te verwijderen voor [!UICONTROL Customer Attributes], moet u:

1. Vermeld het volgende:

   * IMS Org ID
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren
   Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. Als uw marketingteam of interne Adobe-systeembeheerder de IMS Org-id van uw organisatie niet kent, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org-id nodig om aanvragen in te dienen bij de Privacy-API.

1. In [!UICONTROL Privacy Service], kunt u verzoeken van de Toegang en van de Schrapping voorleggen aan de Attributen van de Klant, en de status van bestaande verzoeken controleren.

## Vereiste veldwaarden in [!UICONTROL Customer Attributes] JSON-verzoeken

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

* &quot;verordening&quot;: **ccpa** ( de privacyverordening die op het verzoek van toepassing is )

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
