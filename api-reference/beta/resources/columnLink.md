---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511863"
---
# <a name="columnlink-resource-type"></a>ColumnLink-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | Die eindeutige ID für die Spalte.
| **name**      | string | Der Name der Spalte in diesem Inhaltstyp.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": [
    "Error: /api-reference/beta/resources/columnLink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
