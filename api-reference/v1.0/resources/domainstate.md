---
title: domainState-Ressourcentyp
description: Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.
ms.openlocfilehash: 73a83eddb46b9305a6d74e283bae1c009361195d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018530"
---
# <a name="domainstate-resource-type"></a>domainState-Ressourcentyp

Stellt den Status asynchroner Vorgänge dar, die in einer Domäne geplant sind.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Zeitstempel der letzten Aktivität. Der Wert wird aktualisiert, wenn ein Vorgang geplant, die asynchrone Aufgabe gestartet und der Vorgang abgeschlossen wird. |
| Operation | String | Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification* |
| status | String | Der aktuellen Status des Vorgangs. <br> *Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet. <br> *InProgress*: Der Vorgang wurde gestartet und wird ausgeführt. <br> *Failed*: Ein Fehler ist im Vorgang aufgetreten. |

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->