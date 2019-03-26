---
title: educationAssignmentIndividualRecipient-Ressourcentyp
description: 'Wird innerhalb der Assignment. assignTo-Eigenschaft verwendet. Wenn eine einzelne Empfängerliste festgelegt ist, werden ausgewählte Kursteilnehmer in der Klasse '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799991"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>educationAssignmentIndividualRecipient-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wird innerhalb der [Assignment. assignTo](educationassignment.md) -Eigenschaft verwendet. Wenn eine einzelne Empfängerliste festgelegt ist, erhalten ausgewählte Kursteilnehmer in der Klasse ein Submission-Objekt, wenn die Zuordnung veröffentlicht wird.

Diese Ressource ist eine Unterklasse von [educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|recipients|String collection|Eine Auflistung von IDs der Empfänger.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
