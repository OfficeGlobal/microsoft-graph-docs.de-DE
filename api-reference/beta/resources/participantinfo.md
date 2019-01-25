---
title: Ressourcentyp participantInfo
description: Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528347"
---
# <a name="participantinfo-resource-type"></a>Ressourcentyp participantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung  |
|:---------------|:------------------------------|:-------------|
| [-Identity]       | [identitySet](identityset.md) | Die [IdentitySet](identityset.md) dieser Teilnehmer zugeordnet. |
| languageId     | String                        | Die Sprache-Kultur-Zeichenfolge. |
| Region         | String                        | Region des Teilnehmers. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
