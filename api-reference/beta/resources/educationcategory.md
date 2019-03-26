---
title: educationCategory-Ressourcentyp
description: Eine Kategorie, die auf Zuordnungen angewendet werden kann.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801000"
---
# <a name="educationcategory-resource-type"></a>educationCategory-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Kategorie, die auf Zuordnungen angewendet werden kann.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[EducationCategory abrufen](../api/educationcategory-get.md) | [educationCategory](educationCategory.md) | Abrufen einer vorhandenen **educationCategory**.|
|[Kategorie löschen](../api/educationcategory-delete.md) | Keines | Entfernen einer **educationCategory**.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String|Eindeutiger Bezeichner für die Kategorie.|
|displayName|Zeichenfolge|Eindeutiger Bezeichner für die Kategorie.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
