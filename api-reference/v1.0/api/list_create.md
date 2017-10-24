---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Erstellen einer SharePoint-Liste
ms.openlocfilehash: 7ba657bda38c25ef8f1e5fdda2f7438794e04d2a
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="create-a-new-list"></a>Eine neue Liste erstellen

Erstellen Sie eine neue [Liste][] auf einer [Webseite][].

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|            Berechtigungstyp             | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :------------------------------------------ |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.Manage.All                            |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                              |
| Anwendung                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [list][]-Ressource an.

## <a name="example"></a>Beispiel

Unten sehen Sie ein Beispiel, das die Erstellung einer neuen generischen Liste illustriert.

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

**Hinweis:** Benutzerdefinierte Spalten sind optional.

Zusätzlich zu den hier angegebenen Spalten werden neue Listen mit der in den referenzierten Spalten definierten **Vorlage** erstellt.
Wenn das **Listen**-Facette oder die **Vorlage** nicht angegeben ist, wird für die Liste standardmäßig die `genericList`Vorlage mit der Spalte _Titel_ verwendet.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird ein [list][]-Objekt im Antworttext der neu erstellten Liste zurückgegeben.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

**Hinweis:** Das „Response“-Objekt wurde zwecks besserer Übersichtlichkeit gekürzt.
Der tatsächliche Aufruf gibt die Standardeigenschaften zurück.

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
