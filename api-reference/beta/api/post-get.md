---
title: Beitrag abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können das übergeordnete Element angeben. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0d786734aa59d0048b077d4fa7eae08857da2753
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514012"
---
# <a name="get-post"></a>Beitrag abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Abrufen der Eigenschaften und der Beziehungen eines Beitrags in einem angegebenen Thread. Sie können entweder die übergeordnete Unterhaltung und den Thread oder nur den Thread ohne Verweis auf die übergeordnete Unterhaltung angeben.

Da die **post**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **post**-Instanzen abrufen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.Read.All, Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/post.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
    "id":"AQMkADgAAAIJbQAAAA==",
    "createdDateTime":"2018-01-11T17:36:17Z",
    "lastModifiedDateTime":"2018-01-11T17:36:17Z",
    "importance": "normal",
    "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
    "categories":[

    ],
    "receivedDateTime":"2018-01-11T17:36:17Z",
    "hasAttachments":false,
    "body":{
        "contentType":"html",
        "content":"<html><body></body></html>"
    },
    "from":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    },
    "sender":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    }
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
