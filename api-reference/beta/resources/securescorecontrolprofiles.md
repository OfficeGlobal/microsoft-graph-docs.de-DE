---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063544"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Ressourcentyp secureScoreControlProfiles

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Liste secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.|


## <a name="properties"></a>Eigenschaften

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   Steuerelementname |   String  |   Name des Steuerelements. |
|   title   |   String  |   Titel des Steuerelements.   |
|   controlCategory |   String  |   Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).  |
|   actionType  |   String  |   Steuerelementtyp Aktion (Config überprüfen, Verhalten). |
|   service |   String  |   Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt. |
|   MaxErgebnis |  String  |   Aktuelle abgerufen max Score am angegebenen Datum.   |
|   Tier |  String  |   Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)    |
|   userImpact |    String  | Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).    |
|   implementationCost |    String  |   Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch). |
|   rank |  Int32   |   Microsoft Stapel ranking des Steuerelements.   |
|   Bedrohungen |   Zeichenfolgenauflistung   |   Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing). |
|   veraltet |    Boolesch |   Flag, das angibt, ob ein Steuerelement abgeschrieben wird.   |
|   Wartung |   String  |   Beschreibung, wie das Steuerelement helfen warten. |
|   remediationImpact | String  |   Beschreibung der Auswirkung auf den Benutzer von der Wartung. |
|   actionUrl | String  |   URL zu, in dem das Steuerelement verarbeitet werden kann. |
|   controlStateUpdates |   String  |   Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)). |
|   tenantNote |    String  |   Mandanten kann pro Steuerelement Kommentare (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)) festlegen. |
|   assignedTo |    String  |   Mandanten kann das Steuerelement an eine Person (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)) zuweisen. |
|   updatedBy | String  |   User principal Name des, die der Zustand eines Steuerelements geändert. |

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
