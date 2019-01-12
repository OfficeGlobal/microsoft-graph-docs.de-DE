---
title: Ressourcentyp educationWordResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine Word-Dokument-Ressource. Die Word-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d67f77774b9d3c428fcfd98006115f0459989fdc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948317"
---
# <a name="educationwordresource-resource-type"></a>Ressourcentyp educationWordResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterklasse der [EducationResource](educationresource.md). Hierbei handelt es sich um eine Word-Dokument-Ressource. Die Word-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|Zeichenfolge|Speicherort der Datei auf dem Datenträger.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
