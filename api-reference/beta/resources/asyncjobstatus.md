---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 8c442ad8ff3b23d20e8377a224a3f67b00163f5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820965"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Diese Ressource enthält Informationen zum Status des Fortschritts eines asynchronen Auftrags.

Die folgende API ruft die Rückgabe von **AsyncJobStatus**-Ressourcen auf:

* [Copy Item](../api/driveitem-copy.md)

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname          | Typ   | Beschreibung                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| **percentageComplete** | Gleitkommawert mit doppelter Genauigkeit | Ein Wert zwischen 0 und 100, der den Prozentsatz der Fertigstellung angibt.                          |
| **status**             | Zeichenfolge | Ein Zeichenfolgenwert, der eine Enumeration der möglichen Werte über den Status des Auftrags zuordnet. |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
