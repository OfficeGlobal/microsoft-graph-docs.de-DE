---
title: Ressourcentyp directoryObjectPartnerReference
description: Stellt einen Verweis auf ein Verzeichnisobjekt in einem Partner-Mandanten. Erbt von directoryObject.
ms.openlocfilehash: ebdd7380eaa6b59488aca46120339f7175b640fa
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27224127"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Ressourcentyp directoryObjectPartnerReference

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Verweis auf ein Verzeichnisobjekt in einer Partnerorganisation. Erbt von [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|String| Beschreibung des zurückgegebenen Objekts. Schreibgeschützt. |
|displayName|String| Name des Directory-Objekts zurückgegeben wird, wie die Gruppe oder eine andere Anwendung. Schreibgeschützt. |
|externalPartnerTenantId|Guid| Die Mandanten-ID für den Mandanten Partner. Schreibgeschützt. |
|id|String| Der eindeutige Bezeichner für die Ressource. Geerbt von [directoryObject](directoryobject.md?view=graph-rest-beta). Schreibgeschützt. |
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
