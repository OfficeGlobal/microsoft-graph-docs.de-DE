---
title: Ressourcentyp educationAssignmentGrade
description: " alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses"
ms.openlocfilehash: c9cd043f8887fda9427d7b56cf832001361d03a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063543"
---
# <a name="educationassignmentgrade-resource-type"></a>Ressourcentyp educationAssignmentGrade

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt das **Note** -Objekt in einer Übermittlung an. Dies ist ein abstrakter Typ, der nie instanziiert wird. alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses Typs Ressource. Dieses Objekt wird auch nachverfolgt, die die Benotung Aufgaben verwendet wird. In der **submission.grade** -Eigenschaft wird verwendet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Benutzer, der die Benotung haben. |
|gradedDateTime|DateTimeOffset| Zeitpunkt Uhrzeit auf dieses Objekt zum Absenden die Klasse angewendet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->