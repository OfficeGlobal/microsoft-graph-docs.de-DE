---
title: Ressourcentyp educationSubmissionResource
description: 'Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung. Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.  '
author: dipakboyed
ms.openlocfilehash: bfbf2f522106f5a1e2033898cbb2702223d3e241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361558"
---
# <a name="educationsubmissionresource-resource-type"></a>Ressourcentyp educationSubmissionResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|resource|[educationResource](educationresource.md)|Resource-Objekt.|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->