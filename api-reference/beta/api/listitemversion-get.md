---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines Listenelements – SharePoint-API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 88f442178d3e703c4861e3a6fe5746a7f0c5e8b8
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482105"
---
# <a name="get-a-listitemversion-resource-preview"></a>ListItemVersion-Ressource erhalten (Vorschau)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie die Metadaten für eine bestimmte Version eines [ListItem](../resources/listitem.md) ab.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|            Berechtigungstyp             | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :------------------------------------------ |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.Read.All, Sites.ReadWrite.All         |
| Delegiert (persönliches Microsoft-Konto) | N/V                                         |
| Anwendung                            | Sites.Read.All, Sites.ReadWrite.All         |


## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ListItemVersion](../resources/listitemversion.md)-Objekt im Antworttext zurückgegeben.


## <a name="example"></a>Beispiel

In diesem Beispiel wird eine Version eines listItem abgerufen und die Fields-Auflistung erweitert, um die Werte der Felder im listItem anzufordern.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a>Antwort

Dadurch wird eine Sammlung von Versionen zurückgegeben:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
