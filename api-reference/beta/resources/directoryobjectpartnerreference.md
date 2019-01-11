---
title: Ressourcentyp directoryObjectPartnerReference
description: Stellt einen Verweis auf ein Verzeichnisobjekt in einem Partner-Mandanten. Erbt von directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 46d0f749ac77e7d51e03314e78cfccf494dcc6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884861"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Ressourcentyp directoryObjectPartnerReference

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Verweis auf ein Verzeichnisobjekt in einer Partnerorganisation. Erbt von [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|Zeichenfolge| Beschreibung des zurückgegebenen Objekts. Schreibgeschützt. |
|displayName|Zeichenfolge| Name des Directory-Objekts zurückgegeben wird, wie die Gruppe oder eine andere Anwendung. Schreibgeschützt. |
|externalPartnerTenantId|Guid| Die Mandanten-ID für den Mandanten Partner. Schreibgeschützt. |
|id|Zeichenfolge| Der eindeutige Bezeichner für die Ressource. Geerbt von [directoryObject](directoryobject.md?view=graph-rest-beta). Schreibgeschützt. |
|objectType|Zeichenfolge| Der Typ des Objekts im Mandanten Partner verwiesen wird. Schreibgeschützt. |

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

## <a name="see-also"></a>Weitere Artikel

- [Directory-Objekte aus einer Liste von IDs abrufen](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
