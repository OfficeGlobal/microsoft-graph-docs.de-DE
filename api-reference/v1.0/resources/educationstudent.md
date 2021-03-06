---
title: educationStudent-Ressourcentyp
description: Zusätzliche Informationen, die einem vorhandenen educationUser hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 683a290806f9a70f97bda4aa9429a64578fbcd97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916362"
---
# <a name="educationstudent-resource-type"></a>educationStudent-Ressourcentyp

Zusätzliche Informationen, die einem vorhandenen [educationUser](educationuser.md) hinzugefügt werden, wenn die primaryRole eines Benutzers `student` ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|birthDate|Date| Geburtsdatum des Kursteilnehmers.|
|externalId|String| ID des Kursteilnehmers im Quellsystem.|
|gender|educationGender| Die möglichen Werte sind: `female`, `male`, `other`, `unknownFutureValue`.|
|grade|String|Aktuelle Klassenstufe des Kursteilnehmers.|
|graduationYear|String| Jahr, in dem der Kursteilnehmer die Schule abschließt.|
|studentNumber|String| Kursteilnehmernummer|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
