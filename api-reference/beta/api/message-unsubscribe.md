---
title: 'Meldung: Melden Sie sich ab'
description: Fordert die e-Mail im Namen des angemeldeten Benutzers an eine e-Mail-Verteilerliste kündigen. Verwendet die Informationen in der `List-Unsubscribe` Kopfzeile.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f66c24e2900ca4c881d08a402698dacbaf5af5f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877686"
---
# <a name="message-unsubscribe"></a>Meldung: Melden Sie sich ab

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Fordert die e-Mail im Namen des angemeldeten Benutzers an eine e-Mail-Verteilerliste kündigen. Verwendet die Informationen in der `List-Unsubscribe` Kopfzeile.

Absender einer Nachricht können Adressenlisten benutzerfreundliche durch das Einbeziehen von einer Option für die Empfänger um zu kündigen. Hierzu können sie angeben die `List-Unsubscribe` Kopfzeile in jede Nachricht [RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)folgen.

**Hinweis** Insbesondere für die Aktion **sich abzumelden** funktioniert der Absender muss festlegen `mailto:` und nicht URL-basierte melden Sie sich Informationen ab.

Durch Festlegen dieser Kopfzeile würde Legen Sie auch die **UnsubscribeEnabled** -Eigenschaft der [Nachricht](../resources/message.md) Instanz mit `true`, und die **UnsubscribeData** -Eigenschaft auf die Kopfzeilendaten.

Wenn die **UnsubscribeEnabled** -Eigenschaft einer Nachricht `true`, können Sie die Aktion **Melden Sie sich ab** , um die Benutzer ähnliche zukünftige Nachrichten zu kündigen, wie durch den Absender der Nachricht verwaltet.

Eine Aktion erfolgreich **Kündigen des Abonnements** wird die Nachricht in den Ordner **Gelöschte Objekte** verschoben. Der tatsächliche Ausschluss des Benutzers aus der zukünftigen Mail Verteilung wird vom Absender verwaltet.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.Send    |
|Delegiert (persönliches Microsoft-Konto) | Mail.Send    |
|Anwendung | Mail.Send |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
