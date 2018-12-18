---
title: Ressourcentyp educationSubmissionIndividualRecipient
description: 'Eine Unterklasse der EducationSubmissionRecipient, der angibt, dass eine Übermittlung an eine Person in der Klasse zugewiesen ist.  '
author: dipakboyed
ms.openlocfilehash: 3447c91fe4f387508a3afdf80a7337786d46f860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318802"
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