---
title: Ressourcentyp educationSubmissionResource
description: 'Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung. Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522077"
---
# <a name="educationsubmissionresource-resource-type"></a>Ressourcentyp educationSubmissionResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung. Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Lesen Sie Eigenschaften und die Beziehungen eines **EducationSubmissionResource** -Objekts.|
|[Delete](../api/educationsubmissionresource-delete.md) | Keine |Löschen eines **EducationSubmissionResource** -Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|Zeiger auf die Zuordnung aus der diese Ressource kopiert wurden. Wenn dies null ist, hochgeladen Student die Ressource.|
|id|String| Schreibgeschützt.|
|resource|[educationResource](educationresource.md)|Resource-Objekt|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
