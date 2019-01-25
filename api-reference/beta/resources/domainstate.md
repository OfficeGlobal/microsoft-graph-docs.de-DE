---
title: domainState-Ressourcentyp
description: Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512976"
---
# <a name="domainstate-resource-type"></a>domainState-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Zeitstempel der letzten Aktivität. Der Wert wird aktualisiert, wenn ein Vorgang geplant, die asynchrone Aufgabe gestartet und der Vorgang abgeschlossen wird. |
| Operation | String | Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification* |
| status | Zeichenfolge | Der aktuellen Status des Vorgangs. <br> *Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet. <br> *InProgress*: Der Vorgang wurde gestartet und wird ausgeführt. <br> *Failed*: Ein Fehler ist im Vorgang aufgetreten. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domainstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
