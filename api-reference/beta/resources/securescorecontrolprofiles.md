---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576059"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Ressourcentyp secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.|


## <a name="properties"></a>Eigenschaften

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   Steuerelementname |   String  |   Name des Steuerelements. |
|   title   |   String  |   Titel des Steuerelements.   |
|   controlCategory |   String  |   Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).  |
|   actionType  |   String  |   Steuerelementtyp Aktion (Config überprüfen, Verhalten). |
|   service |   String  |   Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt. |
|   MaxErgebnis |  Gleitkommawert mit doppelter Genauigkeit  |   Aktuelle abgerufen max Score am angegebenen Datum.   |
|   Tier |  String  |   Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)    |
|   userImpact |    String  | Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).    |
|   implementationCost |    String  |   Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch). |
|   rank |  Int32   |   Microsoft Stapel ranking des Steuerelements.   |
|   Bedrohungen |   Zeichenfolgenauflistung   |   Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing). |
|   veraltet |    Boolean |   Flag, das angibt, ob ein Steuerelement abgeschrieben wird.   |
|   Wartung |   String  |   Beschreibung, wie das Steuerelement helfen warten. |
|   remediationImpact | String  |   Beschreibung der Auswirkung auf den Benutzer von der Wartung. |
|   actionUrl | String  |   URL zu, in dem das Steuerelement verarbeitet werden kann. |
|   lastModifiedDateTime |  Zeichenfolge (DateTimeOffset) |   Datum der letzten Änderung |
|   controlStateUpdates |   [SecureScoreControlStateUpdate](securescorecontrolstateupdate.md) -Auflistung |  Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)). |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).|

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
    "title": "String", 
    "azureTenantId": "String (identifier)", 
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
