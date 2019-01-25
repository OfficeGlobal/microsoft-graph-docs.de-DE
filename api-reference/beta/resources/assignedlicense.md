---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der **user**-Entität ist eine Sammlung von assignedLicense.
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524919"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|disabledPlans|GUID-Sammlung|Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.|
|skuId|Guid|Die eindeutige ID der SKU.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
