---
title: Ressourcentyp targetResourceUser
description: Gibt das Benutzerobjekt, das hinzugefügt wurde, aktualisiert oder gelöscht von Administratoren als Teil des Audit-Aktivität an. Die Ressource TargetResource abgeleitet.
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831928"
---
# <a name="targetresourceuser-resource-type"></a>Ressourcentyp targetResourceUser
Gibt das Benutzerobjekt, das hinzugefügt wurde, aktualisiert oder gelöscht von Administratoren als Teil des Audit-Aktivität an. Die Ressource [TargetResource](targetresource.md) abgeleitet.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|userPrincipalName|String|Gibt die eindeutige Id des Benutzers an. Verweist auf die Benutzer-Id für einen bestimmten Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
