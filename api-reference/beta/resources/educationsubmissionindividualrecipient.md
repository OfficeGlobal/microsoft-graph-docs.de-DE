---
title: Ressourcentyp educationSubmissionIndividualRecipient
description: 'Eine Unterklasse der EducationSubmissionRecipient, der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  '
ms.openlocfilehash: 4b74defc1a21427b6169e399262d827561178e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058855"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>Ressourcentyp educationSubmissionIndividualRecipient

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->