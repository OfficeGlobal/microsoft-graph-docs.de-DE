---
title: Ressourcentyp governanceSubject
description: Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832592"
---
# <a name="governancesubject-resource-type"></a>Ressourcentyp governanceSubject

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.


## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ       |Beschreibung|
|:----------|:----------|:----------|
|id         |String     | Die Id des Betreffs.|
|type       |String     |Der Typ des Betreffs. Der Wert kann sein ``User``, ``Group``, und ``ServicePrincipal``.|
|displayName|String     |Der Anzeigename des Betreffs.|
|E-Mail      |String     |Die e-Mail-Adresse des Betreffs Benutzer. Wenn der Betreff in anderen Typen ist, ist leer.|
|principalName|String   |Den Prinzipalnamen des Benutzers Betreff. Wenn der Betreff in anderen Typen ist, ist leer.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
