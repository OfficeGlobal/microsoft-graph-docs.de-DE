---
title: Ressourcentyp targetResourceUser
description: Gibt das Benutzerobjekt, das hinzugefügt wurde, aktualisiert oder gelöscht von Administratoren als Teil des Audit-Aktivität an. Die Ressource TargetResource abgeleitet.
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061429"
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