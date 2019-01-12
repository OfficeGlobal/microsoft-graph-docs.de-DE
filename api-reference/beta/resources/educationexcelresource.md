---
title: Ressourcentyp educationExcelResource
description: 'Eine Unterklasse der EducationResource. Dieser Ressourcentyp stellt ein Excel-Dokument dar.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 11f28da1f2acaecbdd4f57abe8c6c8a03fbac0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982372"
---
# <a name="educationexcelresource-resource-type"></a>Ressourcentyp educationExcelResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterklasse der [EducationResource](educationresource.md). Dieser Ressourcentyp stellt ein Excel-Dokument dar.  
 
>**Hinweis:** Die Excel-Datei muss im Ordner "Resource" die Zuordnung oder Übermittlung-Objekt zu dem diese Ressource gehört zugeordnet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|Zeichenfolge|Zeiger auf das Excel-File-Objekt.|

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
