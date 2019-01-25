---
title: Ressourcentyp privilegedRoleSummary
description: Die Statistiken für eine bestimmte Rolle Zusammenfassung.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513739"
---
# <a name="privilegedrolesummary-resource-type"></a>Ressourcentyp privilegedRoleSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Statistiken für eine bestimmte Rolle Zusammenfassung.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|elevatedCount|int32|Die Anzahl der Benutzer, die die Rolle zugewiesen haben, ist aktiviert.|
|id|string| Der eindeutige Bezeichner für die Rolle. Schreibgeschützt.|
|managedCount|int32|Die Anzahl der Benutzer, die die Rolle zugewiesen haben, aber die Rolle ist deaktiviert.|
|mfaEnabled|Boolescher Wert|**true,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich sind. **false,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich ist.|
|status|string| Mögliche Werte sind: `ok` und `bad`. Der Wert hängt das Verhältnis von (ManagedCount / UsersCount). Wenn das Verhältnis einen vordefinierten Schwellenwert unterschreitet `ok` wird zurückgegeben. Andernfalls `bad` wird zurückgegeben.|
|usersCount|int32|Die Anzahl der Benutzer, die mit der Rolle zugewiesen sind.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
