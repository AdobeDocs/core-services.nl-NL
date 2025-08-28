---
title: Klantenkenmerk ondersteuning voor de California Consumer Privacy Act
description: Meer informatie over ondersteuning voor klantkenmerken voor de California Consumer Privacy Act
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: 106ad989c5eef60dabbe4b82deaed9d87b09d795
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Klantenkenmerk ondersteuning voor de California Consumer Privacy Act

Op deze pagina wordt [!DNL Customer Attributes] support for the California Consumer Privacy Act (CCPA) beschreven.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies en is niet bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de CCPA.

De CCPA is de nieuwe privacywet van Californië, die 1 januari 2020 van kracht is. CCPA verleent de inwoners van Californië nieuwe rechten met betrekking tot hun persoonlijke informatie en legt gegevensbeschermingstaken op aan bepaalde entiteiten die zaken in Californië leiden. De CCPA verleent consumenten het recht om hun persoonlijke gegevens te raadplegen en te wissen en om af te zien van bepaalde activiteiten die als &quot;verkoop&quot; van persoonlijke gegevens aan derden worden aangemerkt.

Als bedrijf, bepaalt u de persoonlijke gegevens die Adobe Experience Cloud verwerkt en namens u opslaat.

Als uw dienstverlener, verleent Adobe Experience Cloud steun voor uw zaken om aan zijn verplichtingen uit hoofde van CCPA te voldoen die op het gebruik van de producten en de diensten van Experience Cloud van toepassing zijn. Deze ondersteuning omvat het beheren van verzoeken om toegang tot en verwijdering van persoonlijke gegevens.

In dit document wordt beschreven hoe [!DNL Customer Attributes] de toegangsrechten en verwijderingsrechten voor CCPA-gegevens van de betrokkenen ondersteunt via de API van Adobe Experience Platform Privacy Service en de gebruikersinterface van Privacy Service.

Voor meer informatie over de diensten van de Privacy van Adobe voor CCPA, zie het [ Centrum van de Privacy van Adobe ](https://www.adobe.com/privacy/ccpa.html).

## Vereiste instellingen voor het verzenden van aanvragen voor [!DNL Customer Attributes]

Als u verzoeken wilt indienen om gegevens voor [!DNL Customer Attributes] te openen en te verwijderen, moet u:

1. Vermeld het volgende:

   * [Organisatie-ID](../../administration/organizations.md)
   * Alias-id van CRS Data Source waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Uw organisatie-id bestaat uit een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. U hebt de id van de organisatie nodig om aanvragen in te dienen bij de API voor privacy. Neem via `gdprsupport@adobe.com` contact op met de klantenservice van Adobe als u de id niet kunt vinden.

1. In [!UICONTROL Privacy Service] kunt u verzoeken om toegang en om verwijdering verzenden naar klantkenmerken en de status van bestaande aanvragen controleren.

## Vereiste veldwaarden in [!DNL Customer Attributes] JSON-verzoeken

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;waarde&quot;: &lt;*de waarde van uw organisatieidentiteitskaart*>

&quot;gebruikers&quot;:

* &quot;sleutel&quot;: &lt;*gewoonlijk de naam van de klant*>
* &quot;actie&quot;: of **toegang** of **schrapping**
* &quot;gebruikers-id&#39;s&quot;:
   * &quot;namespace&quot;: &lt;*identiteitskaart van de Alias van Gegevens van CRS Source*>
   * &quot;type&quot;: **integrationCode**
   * &quot;waarde&quot;: &lt;*identiteitskaart van CRM*>
* &quot;omvat&quot;: **CRS** (dat het product van Adobe is dat op het verzoek van toepassing is)
* &quot;verordening&quot;: **ccpa** (die de privacyverordening is die op het verzoek van toepassing is)

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
