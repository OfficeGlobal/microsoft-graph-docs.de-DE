---
title: Ressourcentyp synchronizationJobRestartCriteria
description: 'Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.'
ms.openlocfilehash: edf5cf258750df72dda2c9754d3543e07fc32e39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058549"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Ressourcentyp synchronizationJobRestartCriteria

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resetScope|String| Durch Trennzeichen getrennte Kombination der folgenden Werte: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`. Verwendung `Full` Wenn Sie alle Optionen möchten.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->