---
title: Aktivität löschen
description: Löschen einer vorhandenen Benutzeraktivität für Ihre app.
ms.openlocfilehash: 9cdd52a2d3f417828e63107465dc28a4791a02e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062847"
---
# <a name="delete-an-activity"></a>Aktivität löschen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Löschen einer vorhandenen Benutzeraktivität für Ihre app.

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
DELETE /me/activities/{id}
```

## <a name="request-headers"></a>Anforderungsheader

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|Authorization | string | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Keine Anforderungstext.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn die Aktivität gelöscht wurde.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->