---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524429"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Ressourcentyp secureScoreControlProfiles

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.|


## <a name="properties"></a>Eigenschaften

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   Steuerelementname |   String  |   Name des Steuerelements. |
|   title   |   String  |   Titel des Steuerelements.   |
| complianceInformation | [ComplianceInformation](complianceinformation.md) -Auflistung | Die Auflistung der Informationen im Zusammenhang mit Compliance secure Score-Steuerelement |
|   controlCategory |   String  |   Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).  |
|   actionType  |   String  |   Steuerelementtyp Aktion (Config überprüfen, Verhalten). |
|   service |   String  |   Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt. |
|   MaxErgebnis |  String  |   Aktuelle abgerufen max Score am angegebenen Datum.   |
|   Ebene |  String  |   Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)    |
|   userImpact |    String  | Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).    |
|   implementationCost |    String  |   Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch). |
|   rank |  Int32   |   Microsoft Stapel ranking des Steuerelements.   |
|   Bedrohungen |   Zeichenfolgenauflistung   |   Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing). |
|   Veraltet |    Boolescher Wert |   Flag, das angibt, ob ein Steuerelement abgeschrieben wird.   |
|   Wartung |   String  |   Beschreibung, wie das Steuerelement helfen warten. |
|   remediationImpact | String  |   Beschreibung der Auswirkung auf den Benutzer von der Wartung. |
|   ActionUrl | String  |   URL zu, in dem das Steuerelement verarbeitet werden kann. |
|   controlStateUpdates |   [SecureScoreControlStateUpdate](securescorecontrolstateupdate.md) -Auflistung |    Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)). |

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
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
