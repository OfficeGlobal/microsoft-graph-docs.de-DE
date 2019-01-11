---
title: Ressourcentyp resourceAccess
description: Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ RequiredResourceAccess ist eine Auflistung von **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862335"
---
# <a name="resourceaccess-resource-type"></a>Ressourcentyp resourceAccess

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ [RequiredResourceAccess](requiredresourceaccess.md) ist eine Auflistung von **ResourceAccess**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Guid|Der eindeutige Bezeichner für eine der [oAuth2Permission](oauth2permission.md) oder [AppRole](approle.md) -Instanzen, die die Anwendung für die Ressource verfügbar macht.|
|type|String|Gibt an, ob die **Id** -Eigenschaft ein [oAuth2Permission](oauth2permission.md) oder ein [AppRole](approle.md)verweist. Mögliche Werte sind "Bereich" oder "Rolle".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
