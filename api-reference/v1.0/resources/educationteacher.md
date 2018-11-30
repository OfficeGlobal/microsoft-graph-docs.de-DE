---
title: educationTeacher-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.
ms.openlocfilehash: 59d3334b7a01b0dd39c357f6598085cd78d1e3ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016869"
---
# <a name="educationteacher-resource-type"></a>educationTeacher-Ressourcentyp

Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `teacher` ist.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalId|String| Die ID der Lehrkraft im Quellsystem.|
|teacherNumber|String|Lehrernummer|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->