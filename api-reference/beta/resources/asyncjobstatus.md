---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482231"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
