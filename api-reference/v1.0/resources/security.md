---
title: Ressourcentyp Sicherheit
description: Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit. Es gibt eine Singleton Sicherheitsressource zurück. Es enthält keine verwendbaren Eigenschaften.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983254"
---
# <a name="security-resource-type"></a>Ressourcentyp Sicherheit

Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit. Es gibt eine Singleton Sicherheitsressource zurück. Es enthält keine verwendbaren Eigenschaften.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [Warnungen auflisten](../api/alert-list.md) | [Warnung](alert.md) -Auflistung | Rufen Sie eine Auflistung der alert-Objekts. |
| [Benachrichtigungen erhalten möchten](../api/alert-get.md) | [Warnung](alert.md) -Auflistung | Rufen Sie ein alert-Objekt. |
| [Aktualisieren von Benachrichtigungen](../api/alert-update.md) | [Warnung](alert.md) -Auflistung | Rufen Sie ein alert-Objekt. |

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|alerts|[Warnung](alert.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Beispiel

**Die Sicherheitsressource** steht im Stamm des Diagramms.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
