---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
ms.openlocfilehash: 9e0f95802f9f75930384ab1534bf4c519fd9cfeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058474"
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
