---
title: Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening
description: Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---


# Klantenkenmerkondersteuning voor algemene gegevensbeschermingsverordening

Op deze pagina wordt beschreven hoe Customer Attributes General Data Protection Regulation (GDPR) ondersteunt.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies of is bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de GDPR.

De [algemene gegevensbeschermingsverordening](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html), die op 25 mei 2018 van kracht is, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens. Het vereenvoudigt ook de regelgeving voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud fungeert als gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe [!UICONTROL Customer Attributes] ondersteuning wordt geboden voor toegang tot en verwijdering van GDPR-gegevens van de betrokkenen via de API van de privacyservice van het Adobe Experience Platform en de gebruikersinterface van de Privacy Service.

Raadpleeg [GDPR en Uw bedrijf](https://www.adobe.com/privacy/general-data-protection-regulation.html)voor meer informatie over wat GDPR voor uw bedrijf betekent.

## Vereiste Opstelling om verzoeken te verzenden [!UICONTROL Customer Attributes]

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
