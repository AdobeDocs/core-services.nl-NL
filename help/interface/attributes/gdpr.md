---
title: 'Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening '
description: Meer informatie over Customer Attributes Support for General Data Protection Regulation
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---


# Klantenkenmerkondersteuning voor algemene gegevensbeschermingsverordening

Op deze pagina wordt beschreven hoe Customer Attributes General Data Protection Regulation (GDPR) ondersteunt.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies of is bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de GDPR.

De [algemene gegevensbeschermingsverordening](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html), die op 25 mei 2018 van kracht is, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens. Het vereenvoudigt ook de regelgeving voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud treedt op als een gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe toegang tot en verwijdering van GDPR-gegevens door de betrokkenen worden [!UICONTROL Customer Attributes] ondersteund met de API van Adobe Experience Platform Privacy Service en de gebruikersinterface van de Privacy Service.

Raadpleeg [GDPR en Uw bedrijf](https://www.adobe.com/nl/privacy/general-data-protection-regulation.html)voor meer informatie over wat GDPR voor uw bedrijf betekent.

## Vereiste Opstelling om verzoeken te verzenden [!UICONTROL Customer Attributes]

Als u verzoeken wilt indienen om gegevens te openen en te verwijderen voor [!UICONTROL Customer Attributes], moet u:

1. Vermeld het volgende:

   * IMS-organisatie-id
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. Als uw marketingteam of interne beheerder van het Adobe-systeem de IMS Org-id van uw organisatie niet kent, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org-id nodig om aanvragen in te dienen bij de Privacy-API.

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

* &quot;include&quot;: **CRS** (het product van de Adobe dat op het verzoek van toepassing is)

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

## Gegevensvelden die worden geretourneerd voor toegangsverzoeken

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
