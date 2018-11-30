---
title: 'Benutzer: InvalidateAllRefreshTokens'
description: Alle des Benutzers Aktualisierungstoken einstufen Applications (als auch Session-Cookies im Browser des Benutzers), die Benutzereigenschaft **RefreshTokensValidFromDateTime** auf das aktuelle Datum-Uhrzeit zurücksetzen ungültig macht. Dieser Vorgang wird in der Regel (durch den Benutzer oder Administrator) ausgeführt, wenn der Benutzer einem verlorenen oder gestohlenen Gerät verfügt.  Dieser Vorgang würde Zugriff auf die Organisation Daten über Anwendungen auf dem Gerät zugegriffen werden, ohne dass der Benutzer zunächst eine erneute Anmeldung erforderlich wird verhindern. Tatsächlich würden diese Operation erzwingen, dass den Benutzer erneut für alle Anwendungen anmelden, die sie zuvor, zugestimmt haben unabhängig vom Gerät.
ms.openlocfilehash: 23743c4bc372193a5478d79432b7bb4e0a9ec4ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064889"
---
# <a name="user-invalidateallrefreshtokens"></a>Benutzer: InvalidateAllRefreshTokens

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Alle des Benutzers Aktualisierungstoken einstufen Applications (als auch Session-Cookies im Browser des Benutzers), die Benutzereigenschaft **RefreshTokensValidFromDateTime** auf das aktuelle Datum-Uhrzeit zurücksetzen ungültig macht. Dieser Vorgang wird in der Regel (durch den Benutzer oder Administrator) ausgeführt, wenn der Benutzer einem verlorenen oder gestohlenen Gerät verfügt.  Dieser Vorgang würde Zugriff auf die Organisation Daten über Anwendungen auf dem Gerät zugegriffen werden, ohne dass der Benutzer zunächst eine erneute Anmeldung erforderlich wird verhindern. Tatsächlich würden diese Operation erzwingen, dass den Benutzer erneut für alle Anwendungen anmelden, die sie zuvor, zugestimmt haben unabhängig vom Gerät.

Für Entwickler Wenn die Anwendung versucht, ein Token Delegierter Zugriff für diesen Benutzer mithilfe einer ungültig Aktualisierungstoken lösen Sie, erhalten die Anwendung einen Fehler. In diesem Fall muss die Anwendung erwirbt ein neues Aktualisierungstoken durch eine Anforderung an den Endpunkt autorisieren, in der den Benutzer zur Anmeldung bei erzwungen wird.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

+ Für eine Anwendung an Benutzer Applikationen für ungültig erklärt die signierte zulassen, die sie zum zugestimmt haben: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All
+ Für eine Anwendung an Applications ungültig ein Administrator kann ein Benutzer zugestimmt hat: Directory.ReadWrite.All, Directory.AccessAsUser.All

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Dieser Vorgang hat keine Anforderung Inhalt.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
