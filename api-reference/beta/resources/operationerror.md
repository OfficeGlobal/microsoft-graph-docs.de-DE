---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526130"
---
# <a name="operationerror-resource-type"></a>Ressourcentyp operationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fehler in [TeamsAsyncOperation](teamsasyncoperation.md)beschreibt.

## <a name="operationerror-properties"></a>OperationError Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|code|Zeichenfolge (schreibgeschützt)|Fehlercode Vorgang.|
|message|Zeichenfolge (schreibgeschützt)|Vorgang Fehlermeldung angezeigt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
