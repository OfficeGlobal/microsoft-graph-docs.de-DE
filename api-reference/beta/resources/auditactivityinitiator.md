---
title: Ressourcentyp auditActivityInitiator
description: Identität das Resource-Objekt, das die Aktivität initiiert. Der Initiator kann es sich um einen Benutzer, eine app oder eines Systems (die als eine app betrachtet wird)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884609"
---
# <a name="auditactivityinitiator-resource-type"></a>Ressourcentyp auditActivityInitiator
Identität das Resource-Objekt, das die Aktivität initiiert. Der Initiator kann es sich um einen Benutzer, eine app oder eines Systems (die als eine app betrachtet wird)



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|App|[appIdentity](appidentity.md)|Wenn die Ressource die Aktivität Initiieren einer app ist, gibt diese Eigenschaft alle app weiterführende Informationen wie AppId, Name, ServicePrincipalId Name.|
|user|[Benutzeridentität](useridentity.md)|Wenn die Ressource die Aktivität Initiieren eines Benutzers ist, gibt diese Eigenschaft alle Benutzer weiterführende Informationen wie Benutzer-ID, Name, userPrincipalName.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
