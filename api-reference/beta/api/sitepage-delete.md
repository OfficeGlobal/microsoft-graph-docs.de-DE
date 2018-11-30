---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Löschen einer Seite aus einer SharePoint-Website
ms.openlocfilehash: c537acec2e205ffd556a35789f75be95e2b94017
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060062"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>Löschen der Seite aus der Liste Website Seiten einer Website

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Entfernt eine [SitePage][] aus der Website-Seiten- [Liste][] in einer [Website][].

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Um ein Element zu löschen, muss der Benutzer die Anwendung Schreibzugriff auf das Element, das gelöscht werden erteilt haben.

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name       | Wert | Beschreibung
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.

## <a name="request-body"></a>Anforderungstext

Bei dieser Methode wird kein Anforderungstext angegeben.
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a>Antwort

Wenn erfolgreich ist, dieses Anrufs gibt eine `204 No Content` Antwort, um anzugeben, dass die Ressource wurde gelöscht, und es nothing wurde zurückgegeben.

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>Anforderung

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>Antwort

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
