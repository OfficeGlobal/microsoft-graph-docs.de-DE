---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Löschen einer Seite aus einer SharePoint-Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513025"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>Löschen der Seite aus der Liste Website Seiten einer Website

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
