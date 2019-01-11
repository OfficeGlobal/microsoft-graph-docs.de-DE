---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Löschen eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.openlocfilehash: 71be680ae2d29d083d06c9d18aa79675ebdd01dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849280"
---
# <a name="delete-an-item-from-a-list"></a>Element aus einer Liste löschen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Entfernt ein Element aus einer [Liste][].

[list]: ../resources/list.md

## <a name="permissions"></a>Berechtigungen

Damit ein Element gelöscht werden kann, muss der Benutzer der Anwendung Schreibzugriff auf das zu löschende Element gewährt haben.

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name       | Wert | Beschreibung
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.

## <a name="request-body"></a>Anforderungstext

Bei dieser Methode wird kein Anforderungstext angegeben.

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
