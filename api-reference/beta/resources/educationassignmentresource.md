---
title: Ressourcentyp educationAssignmentResource
description: Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource wird
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529229"
---
# <a name="educationassignmentresource-resource-type"></a>Ressourcentyp educationAssignmentResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource in der Studentenübermittlung kopiert werden.  Wenn das Objekt nicht kopiert wird, sehen Studenten einen Link zu der Ressource für die Zuordnung. Die Student möglich so aktualisieren Sie diese Ressource nicht. Hierbei handelt es sich um Handzetteln aus der Schulungsleiter in den Teilnehmern nothing in aktiviert werden. Wenn die Ressource verteilt ist, erhält jeder Student eine Kopie dieser Ressource in der Ressourcenliste ihrer Einreichung. Studenten werden ihre Kopie ändern und zur Benotung übermitteln können.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Lesen Sie Eigenschaften und die Beziehungen eines **EducationAssignmentResource** -Objekts.|
|[Update](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |Aktualisieren eines **EducationAssignmentResource** -Objekts. |
|[Delete](../api/educationassignmentresource-delete.md) | Keine |Löschen eines **EducationAssignmentResource** -Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolescher Wert|Gibt an, ob diese Ressource in jeder Studentenübermittlung für Änderung und Übermittlung kopiert werden sollen.|
|id|String| Die ID der Ressource. Schreibgeschützt.|
|resource|[educationResource](educationresource.md)|Resource-Objekt, das diese Zuordnung zugeordnet wurde.|

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
