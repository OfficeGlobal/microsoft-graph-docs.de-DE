---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
localization_priority: Normal
ms.openlocfilehash: 423f426df92e99754af0abf4c9c8088eea61d5ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890293"
---
# <a name="operationerror-resource-type"></a>Ressourcentyp operationError

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
