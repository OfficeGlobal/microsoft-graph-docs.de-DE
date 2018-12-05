---
title: Audio Routinggruppe löschen
description: Löschen der angegebenen AudioRoutingGroup.
ms.openlocfilehash: cb4b4c2cf3f7023332acd443c63463d5251963ad
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/05/2018
ms.locfileid: "27155991"
---
# <a name="delete-audio-routing-group"></a>Audio Routinggruppe löschen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Löschen der angegebenen [AudioRoutingGroup](../resources/audioroutinggroup.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)  |
| :-------------- | :------------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Nicht unterstützt        |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt        |
| Anwendung     | Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a>Anforderungsheader
| Name          | Beschreibung               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Das folgende Beispiel zeigt die Antwort.

<!-- {
  "blockType": "request",
  "name": "delete_audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a>Antwort

> **Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
