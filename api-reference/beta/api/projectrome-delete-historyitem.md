---
title: Löschen einer historyItem
description: Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.
localization_priority: Normal
ms.openlocfilehash: d9468034f3a98e949eeb9f2da28c4a74c42cd991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834979"
---
# <a name="delete-a-historyitem"></a>Löschen einer historyItem

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | UserActivity.ReadWrite.CreatedByApp    |
|Delegiert (persönliches Microsoft-Konto) | UserActivity.ReadWrite.CreatedByApp    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a>Anforderungsheader

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Authorization | string | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Keine Anforderungstext.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn das Historienelement gelöscht wurde.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
