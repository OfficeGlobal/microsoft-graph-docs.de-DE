---
title: Diagnose Ressourcentyp
description: Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.
ms.openlocfilehash: 29e30d44a9fde91b79778042be19461b880216ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063950"
---
# <a name="diagnostic-resource-type"></a>Diagnose Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|message|String|Die Nachricht, beschreibt die Bedingung, die den Fehler oder eine Warnung ausgelöst.|
|url|String|Die Verknüpfung mit der Dokumentation für dieses Problem.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->