---
title: Ressourcentyp directoryObjectPartnerReference
description: Stellt einen Verweis auf ein Verzeichnisobjekt in einem Partner-Mandanten. Erbt von directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba72f70a29e778127454ec3bd4f259331d1fe4c5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570744"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Ressourcentyp directoryObjectPartnerReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Verweis auf ein Verzeichnisobjekt in einer Partnerorganisation. Erbt von [directoryObject](../resources/directoryobject.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|String| Beschreibung des zurückgegebenen Objekts. Schreibgeschützt. |
|displayName|String| Name des Directory-Objekts zurückgegeben wird, wie die Gruppe oder eine andere Anwendung. Schreibgeschützt. |
|externalPartnerTenantId|Guid| Die Mandanten-ID für den Mandanten Partner. Schreibgeschützt. |
|id|String| Der eindeutige Bezeichner für die Ressource. Geerbt von [directoryObject](../resources/directoryobject.md). Schreibgeschützt. |
|objectType|String| Der Typ des Objekts im Mandanten Partner verwiesen wird. Schreibgeschützt. |

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

- [Directory-Objekte aus einer Liste von IDs abrufen](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
