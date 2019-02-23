---
title: directoryObjectPartnerReference-Ressourcentyp
description: Stellt einen Verweis auf ein Directory-Objekt in einem Partner Mandanten dar. Erbt von directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b84b7447d689759444e9cfd99982857eafa71eb
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/23/2019
ms.locfileid: "30224129"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference-Ressourcentyp

Stellt einen Verweis auf ein Directory-Objekt in einer Partnerorganisation dar. Erbt von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|Zeichenfolge| Beschreibung des zurückgegebenen Objekts. Schreibgeschützt. |
|displayName|String| Name des Verzeichnisobjekts, das zurückgegeben wird, wie Gruppe oder Anwendung. Schreibgeschützt. |
|externalPartnerTenantId|Guid| Die Mandanten-ID für den Partner Mandanten. Schreibgeschützt. |
|id|string| Der eindeutige Bezeichner für die Ressource. Geerbt von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Schreibgeschützt. |
|objectType|String| Der Typ des referenzierten Objekts im Partner Mandanten. Schreibgeschützt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>Siehe auch

- [Directory-Objekte aus einer Liste von IDs abrufen](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
