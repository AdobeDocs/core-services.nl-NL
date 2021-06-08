---
title: 'Klantkenmerken Ondersteuning voor algemene gegevensbeschermingsverordening '
description: Meer informatie over Customer Attributes Support for General Data Protection Regulation
feature: Klantkenmerken
topic: Beheer
role: Administrator
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: c7ed1324015beb7ebcf7a4ee21b05601e36e608f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 1%

---

# Klantenkenmerkondersteuning voor algemene gegevensbeschermingsverordening

Op deze pagina wordt beschreven hoe [!UICONTROL Customer Attributes] algemene gegevensbeschermingsverordening (GDPR) ondersteunt.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies of is bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de GDPR.

De [Algemene gegevensbeschermingsverordening](https://business.adobe.com/privacy/general-data-protection-regulation.html), een wet die van kracht is op 25 mei 2018, geeft alle personen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle op hun persoonsgegevens. Het vereenvoudigt ook de regelgeving voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud treedt op als een gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe [!UICONTROL Customer Attributes] de toegang tot en het verwijderen van GDPR-gegevens van de betrokkenen via de API van Adobe Experience Platform Privacy Service en de gebruikersinterface van de Privacy Service ondersteunt.

Voor meer informatie over wat GDPR voor uw zaken betekent, zie [GDPR en Uw Zaken](https://business.adobe.com/privacy/general-data-protection-regulation.html).

## Vereiste installatie voor het verzenden van aanvragen voor [!UICONTROL Customer Attributes]

Als u verzoeken wilt indienen om gegevens voor [!UICONTROL Customer Attributes] te openen en te verwijderen, moet u:

1. Vermeld het volgende:

   * IMS-organisatie-id
   * Alias-id van CRS-gegevensbron waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Een IMS-organisatie-id is een alfanumerieke tekenreeks van 24 tekens die wordt toegevoegd met @AdobeOrg. Als uw marketingteam of interne beheerder van het Adobe-systeem de IMS Org-id van uw organisatie niet kent, neemt u contact op met de klantenservice van Adobe op gdprsupport@adobe.com. U hebt de IMS Org ID nodig om aanvragen in te dienen bij de Privacy API.

1. In [!UICONTROL Privacy Service], kunt u verzoeken van de Toegang en van de Schrapping aan de Attributen van de Klant voorleggen, en de status van bestaande verzoeken controleren.

## Vereiste veldwaarden in JSON-aanvragen [!UICONTROL Customer Attributes]

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
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```