---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380583"
---
# <a name="securescorecontrolprofiles-resource-type"></a>Ressourcentyp secureScoreControlProfiles

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.|


## <a name="properties"></a>Eigenschaften

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   azureTenantId   |   Zeichenfolge  |   GUID-Zeichenfolge für Mandanten-ID ein.  |
|   Steuerelementname |   Zeichenfolge  |   Name des Steuerelements. |
|   title   |   Zeichenfolge  |   Titel des Steuerelements.   |
| complianceInformation | [ComplianceInformation](complianceinformation.md) -Auflistung | Die Auflistung der Informationen im Zusammenhang mit Compliance secure Score-Steuerelement |
|   controlCategory |   Zeichenfolge  |   Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).  |
|   actionType  |   String  |   Steuerelementtyp Aktion (Config überprüfen, Verhalten). |
|   service |   Zeichenfolge  |   Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt. |
|   MaxErgebnis |  Zeichenfolge  |   Aktuelle abgerufen max Score am angegebenen Datum.   |
|   Tier |  Zeichenfolge  |   Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)    |
|   userImpact |    Zeichenfolge  | Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).    |
|   implementationCost |    Zeichenfolge  |   Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch). |
|   rank |  Int32   |   Microsoft Stapel ranking des Steuerelements.   |
|   Bedrohungen |   Zeichenfolgenauflistung   |   Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing). |
|   veraltet |    Boolescher Wert |   Flag, das angibt, ob ein Steuerelement abgeschrieben wird.   |
|   Wartung |   Zeichenfolge  |   Beschreibung, wie das Steuerelement helfen warten. |
|   remediationImpact | Zeichenfolge  |   Beschreibung der Auswirkung auf den Benutzer von der Wartung. |
|   actionUrl | Zeichenfolge  |   URL zu, in dem das Steuerelement verarbeitet werden kann. |
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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
