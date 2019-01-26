---
title: Ressourcentyp sharingDetail
description: 'Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 380db80f120b29a0d1dca1a4b052679e483bc6f7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571037"
---
# <a name="sharingdetail-resource-type"></a>Ressourcentyp sharingDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält. 

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| Das Datum und die Zeit, die die Datei zuletzt freigegeben wurde. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`. Schreibgeschützt.  |
| sharingSubject        | String          | Der Betreff, mit dem das Dokument freigegeben wurde. |
| sharingType             | String        | Bestimmt, wie das Dokument freigegeben wurde, kann durch "Link", "Anlage", "Group", "Site" sein.     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Der Benutzer, die das Dokument freigegeben.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
