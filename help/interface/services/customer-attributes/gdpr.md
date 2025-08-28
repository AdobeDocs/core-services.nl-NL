---
title: '[!DNL Customer attributes] Ondersteuning voor algemene gegevensbeschermingsverordening'
description: Meer informatie over ondersteuning van klantkenmerken voor algemene gegevensbeschermingsverordening
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: 21120abb5ab0fcc8d556012851548f39f3875038
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# [!DNL Customer Attributes] ondersteuning voor algemene gegevensbeschermingsverordening

Op deze pagina wordt beschreven hoe [!DNL Customer Attributes] General Data Protection Regulation (GDPR) ondersteunt.

>[!IMPORTANT]
>
>De inhoud van dit document is geen juridisch advies of is bedoeld ter vervanging van juridisch advies. Raadpleeg uw juridisch adviseur voor advies over de GDPR.

De [ Algemene Verordening van de Bescherming van Gegevens ](https://business.adobe.com/privacy/general-data-protection-regulation.html), een wet in werking 25 mei, 2018, geeft alle individuen (betrokkenen) binnen de grenzen van de Europese Unie (EU) controle van hun persoonsgegevens. Het vereenvoudigt ook de regelgeving voor het internationale bedrijfsleven. Deze wet is van toepassing op alle ondernemingen (voor de verwerking van persoonsgegevens verantwoordelijke personen) die goederen of diensten aanbieden, het gedrag van personen binnen de grenzen van de EU volgen of persoonsgegevens verzamelen op het tijdstip waarop hun persoonsgegevens worden verwerkt, ongeacht de bedrijfslocatie van de voor de verwerking verantwoordelijke.

Adobe Experience Cloud treedt op als een gegevensverwerker voor persoonlijke gegevens die het ontvangt en opslaat namens zijn klanten. Als gegevenscontroller bepaalt u de persoonlijke gegevens die Adobe Experience Cloud voor u verwerkt en opslaat.

In dit document wordt beschreven hoe [!DNL Customer Attributes] de toegang tot en het verwijderen van GDPR-gegevens van de betrokkenen via de Adobe Experience Platform Privacy Service API en de gebruikersinterface van Privacy Service ondersteunt.

Voor meer informatie over wat GDPR voor uw zaken betekent, zie [ GDPR en Uw Zaken ](https://business.adobe.com/privacy/general-data-protection-regulation.html).

## Vereiste instellingen voor het verzenden van aanvragen voor [!DNL Customer Attributes]

Als u verzoeken wilt indienen om gegevens voor [!DNL Customer Attributes] te openen en te verwijderen, moet u:

1. Vermeld het volgende:

   * [Organisatie-ID](../../administration/organizations.md)
   * Alias-id van CRS Data Source waarop u wilt reageren
   * CRM-id van het profiel waarop u wilt reageren

   Uw [ organisatieidentiteitskaart ](../../administration/organizations.md) is een 24 karakter alfanumeriek koord dat met @AdobeOrg wordt toegevoegd. U hebt de id van de organisatie nodig om aanvragen in te dienen bij de API voor privacy. Neem via `gdprsupport@adobe.com` contact op met de klantenservice van Adobe als u de id niet kunt vinden.

1. In [!UICONTROL Privacy Service] kunt u aanvragen voor toegang en verwijderen indienen bij [!DNL Customer Attributes] en de status van bestaande aanvragen controleren.

## Vereiste veldwaarden in [!DNL Customer Attributes] JSON-aanvragen

&quot;bedrijfcontext&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;waarde&quot;: &lt;*uw waarde van identiteitskaart IMS die van de Org*>

&quot;gebruikers&quot;:

* &quot;sleutel&quot;: &lt;*gewoonlijk de naam van de klant*>
* &quot;actie&quot;: of **toegang** of **schrapping**
* &quot;gebruikers-id&#39;s&quot;:
   * &quot;namespace&quot;: &lt;*identiteitskaart van de Alias van Gegevens van CRS Source*>
   * &quot;type&quot;: **integrationCode**
   * &quot;waarde&quot;: &lt;*identiteitskaart van CRM*>
* &quot;omvat&quot;: **CRS** (dat het product van Adobe is dat op het verzoek van toepassing is)
* &quot;verordening&quot;: **gdpr** (die de privacyverordening is die op het verzoek van toepassing is)

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
