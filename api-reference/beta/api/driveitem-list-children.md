---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Auflisten der Inhalte eines Ordners
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a5d31d39b393725c325a75b6a8ba7e52516938b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513130"
---
# <a name="list-children-of-a-driveitem"></a>Untergeordnete Elemente eines DriveItem auflisten

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Auflistung von [DriveItems](../resources/driveitem.md) im **untergeordneten** Verhältnis eines DriveItem zurückgeben.

Ressourcen des Typs „DriveItems“ mit einer Facette des Typs **folder** oder **package**, die einen anderen Wert als „null“ hat, können eine oder mehrere untergeordnete Ressourcen des Typs „DriveItems“ haben.


## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

### <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Headername     | Wert | Beschreibung                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | etag  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="examples"></a>Beispiele

### <a name="list-children-in-the-root-of-the-current-users-drive"></a>Untergeordnete Elemente im Stammverzeichnis des Laufwerk des aktuellen Benutzers auflisten

Wenn Sie Dateien aus dem Stammordner des Laufwerks abrufen möchten, wenden Sie die `root`-Beziehung auf das Laufwerk an und greifen Sie dann auf die untergeordnete Beziehung zu.

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a>Untergeordnete Elemente eines DriveItem mit einer bekannten ID auflisten

Wenn Sie Dateien aus dem Stammordner des Laufwerks abrufen möchten, wenden Sie die `root`-Beziehung auf das Laufwerk an und greifen Sie dann auf die untergeordnete Beziehung zu.

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a>Untergeordnete Elemente eines DriveItem mit einem bekannten Pfad auflisten

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird die Liste der Elemente in der Auflistung der untergeordneten Elemente des Zielelements zurückgegeben.
Die Auflistung untergeordneter Elemente besteht aus [driveItem][item-resource]-Ressourcen.

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

**Hinweis:** Wenn eine Auflistung die Standardseitengröße (200 Artikel) überschreitet, wird die Eigenschaft **@odata.nextLink** in der Antwort zurückgegeben, damit angezeigt wird, dass mehr Elemente zur Verfügung, und die Anfrage-URL für die nächste Seite von Elementen zurückzugeben.

Sie können die Seitengröße über [Optionale Abfragezeichenfolge-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) steuern.

### <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
