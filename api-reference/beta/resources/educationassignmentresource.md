---
title: Ressourcentyp educationAssignmentResource
description: Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource wird
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991349"
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
|distributeForStudentWork|Boolescher Wert|Gibt an, ob diese Ressource in jeder Studentenübermittlung für Änderung und Übermittlung kopiert werden sollen.|
|id|Zeichenfolge| Die ID der Ressource. Schreibgeschützt.|
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
