---
title: Ressourcentyp educationExcelResource
description: 'Eine Unterklasse der EducationResource. Dieser Ressourcentyp stellt ein Excel-Dokument dar.  '
author: mmast-msft
ms.openlocfilehash: 427de6fac1f5f4ad63de8286e2714dd8fad472f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315939"
---
# <a name="educationexcelresource-resource-type"></a>Ressourcentyp educationExcelResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterklasse der [EducationResource](educationresource.md). Dieser Ressourcentyp stellt ein Excel-Dokument dar.  
 
>**Hinweis:** Die Excel-Datei muss im Ordner "Resource" die Zuordnung oder Übermittlung-Objekt zu dem diese Ressource gehört zugeordnet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|String|Zeiger auf das Excel-File-Objekt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->