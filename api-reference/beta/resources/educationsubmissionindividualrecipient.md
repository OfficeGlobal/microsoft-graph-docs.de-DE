---
title: Ressourcentyp educationSubmissionIndividualRecipient
description: 'Eine Unterklasse der EducationSubmissionRecipient, der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519185"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>Ressourcentyp educationSubmissionIndividualRecipient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Unterklasse der [EducationSubmissionRecipient](educationsubmissionrecipient.md) , der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|userId|String|Benutzer-ID des Benutzers, dem die Übermittlung zugewiesen ist.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
