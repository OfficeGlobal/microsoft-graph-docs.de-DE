---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Erstellen einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 88b12ebbe56a3e57b441581ba319734edbe9e5c5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482140"
---
# <a name="create-a-new-list"></a>Eine neue Liste erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie eine neue [Liste][] auf einer [Webseite][].

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|            Berechtigungstyp             | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :------------------------------------------ |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.Manage.All                            |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                              |
| Anwendung                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [liste][]-Ressource an.

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

Wenn die Methode erfolgreich verläuft, wird ein [liste][]-Objekt im Antworttext der neu erstellten Liste zurückgegeben.

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

[liste]: ../resources/list.md
[Webseite]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/list-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
