---
title: Ressourcentyp governanceRoleSetting
description: " Regel, und So weiter."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508167"
---
# <a name="governancerolesetting-resource-type"></a>Ressourcentyp governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Reihe von Konfigurationen auf jede Rollendefinition, die ausgewertet werden, wenn rollenzuweisungen erstellt oder geändert werden muss. Beispielsweise können Einstellungen für Serverrollen Regel "Dauer maximale Zuordnung", "Mehrstufiger Authentifizierung das erforderlich für die Aktivierung" Regel usw. enthalten.

## <a name="methods"></a>Methoden

| Methode          | Rückgabetyp |Beschreibung|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung|Eine Auflistung von Einstellungen für Serverrollen auf eine Ressource aufgelistet.|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Lesen Sie Eigenschaften und Beziehungen einer Rolle-Einstellung.|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Aktualisieren einer Einstellungsobjekt für die Rolle. |

## <a name="properties"></a>Eigenschaften
|Eigenschaft               |Typ                                      |Beschreibung|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |Die Id des der RoleSetting.|
|resourceId           |Zeichenfolge                                  |Erforderlich. Die Id der Ressource, der die Einstellung der Rolle zugeordnet ist.|
|roleDefinitionId     |Zeichenfolge                                  |Erforderlich. Die Id der Rollendefinition, der die Einstellung der Rolle zugeordnet ist.|
|isDefault            |Boolescher Wert                                 |Schreibgeschützt. Gibt an, ob die RoleSetting eine standardmäßige RoleSetting ist|
|lastUpdatedDateTime  |DateTimeOffset                          |Schreibgeschützt. Der Zeitpunkt, wann die Rolle Einstellung zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|lastUpdatedBy        |String                                  |Schreibgeschützt. Der Anzeigename des Administrators, der die RoleSetting zuletzt aktualisiert.|
|adminEligibleSettings|[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung|Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen.|
|adminMemberSettings  |[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung|Die Einstellungen, die ausgewertet werden, wenn ein Administrator versucht, eine direkte rollenzuweisung hinzufügen.|
|userEligibleSettings |[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung|Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, eine Aufgabe zu auswählbaren Rolle hinzufügen. Die Einstellung wird derzeit nicht unterstützt.|
|userMemberSettings   |[GovernanceRuleSetting](../resources/governancerulesetting.md) -Auflistung|Die Einstellungen, die ausgewertet werden, wenn ein Benutzer versucht, seine rollenzuweisung aktivieren.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Schreibgeschützt. Die zugeordneten Ressource für diese Rolle-Einstellung.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Schreibgeschützt. Die Rollendefinition, die erzwungen wird mit dieser Einstellung Rolle. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
