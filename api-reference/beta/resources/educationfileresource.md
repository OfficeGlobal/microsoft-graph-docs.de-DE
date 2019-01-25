---
title: Ressourcentyp educationFileResource
description: Eine Unterklasse der EducationResource, die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520795"
---
# <a name="educationfileresource-resource-type"></a>Ressourcentyp educationFileResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Unterklasse der [EducationResource](educationresource.md) , die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|String|Speicherort auf dem Datenträger den File-Ressource.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
