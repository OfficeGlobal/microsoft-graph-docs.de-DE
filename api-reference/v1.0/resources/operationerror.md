---
title: Ressourcentyp operationError
description: Fehler in TeamsAsyncOperation beschreibt.
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018995"
---
# <a name="operationerror-resource-type"></a>Ressourcentyp operationError



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
