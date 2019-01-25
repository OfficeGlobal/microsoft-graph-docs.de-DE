---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: 5e3b7cbf752d3ddb2c4b7bde3981d2a443028b92
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512619"
---
# <a name="deleteaction-resource-type"></a>DeleteAction-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wenn eine **DeleteAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element gelöscht hat.

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung
|:--------------|:-------|:----------------------------------------------------
| name          | string | Der Name des Elements, das gelöscht wurde.
| objectType    | string | `File`oder `Folder`, je nach Typ des gelöschten Elements.

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleteaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
