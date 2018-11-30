---
title: Ressourcentyp educationAssignmentResource
description: Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource wird
ms.openlocfilehash: 6907af5e4408248487b118c390bb2ec209700124
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062224"
---
# <a name="educationassignmentresource-resource-type"></a>Ressourcentyp educationAssignmentResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|distributeForStudentWork|Boolesch|Gibt an, ob diese Ressource in jeder Studentenübermittlung für Änderung und Übermittlung kopiert werden sollen.|
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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
