---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines Listenelements – SharePoint-API
localization_priority: Normal
ms.openlocfilehash: 7f009eb006e44dd2f8e25052b0326ffc92243c7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881606"
---
# <a name="get-a-listitemversion-resource-preview"></a>ListItemVersion-Ressource erhalten (Vorschau)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
