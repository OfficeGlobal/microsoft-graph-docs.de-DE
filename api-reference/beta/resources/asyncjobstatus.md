---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: ee7cc92bff47edc3a1a15b5f27cb2f5afe061d4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510211"
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
