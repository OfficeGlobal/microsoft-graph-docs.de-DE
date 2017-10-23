---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Auflisten der Inhalte eines Ordners
ms.openlocfilehash: e4c8f7b66333d739aeeaff9a8b92c0088d2fde0b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="2b7fd-102">Untergeordnete Elemente eines DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="2b7fd-102">List children of a driveItem</span></span>

<span data-ttu-id="2b7fd-103">Eine Auflistung von [DriveItems](../resources/driveitem.md) im **untergeordneten** Verhältnis eines DriveItem zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="2b7fd-104">Ressourcen des Typs „DriveItems“ mit einer Facette des Typs **folder** oder **package**, die einen anderen Wert als „null“ hat, können eine oder mehrere untergeordnete Ressourcen des Typs „DriveItems“ haben.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="2b7fd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b7fd-105">Permissions</span></span>

<span data-ttu-id="2b7fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b7fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b7fd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b7fd-108">Permission type</span></span>      | <span data-ttu-id="2b7fd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b7fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7fd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b7fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b7fd-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7fd-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b7fd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b7fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b7fd-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7fd-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b7fd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b7fd-114">Application</span></span> | <span data-ttu-id="2b7fd-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7fd-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b7fd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b7fd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b7fd-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2b7fd-117">Optional query parameters</span></span>

<span data-ttu-id="2b7fd-118">Diese Methode unterstützt `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="2b7fd-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b7fd-119">Optional request headers</span></span>

| <span data-ttu-id="2b7fd-120">Headername</span><span class="sxs-lookup"><span data-stu-id="2b7fd-120">Header name</span></span>     | <span data-ttu-id="2b7fd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2b7fd-121">Value</span></span> | <span data-ttu-id="2b7fd-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b7fd-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2b7fd-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="2b7fd-123">_if-none-match_</span></span> | <span data-ttu-id="2b7fd-124">etag</span><span class="sxs-lookup"><span data-stu-id="2b7fd-124">etag</span></span>  | <span data-ttu-id="2b7fd-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="2b7fd-126">Beispiele</span><span class="sxs-lookup"><span data-stu-id="2b7fd-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="2b7fd-127">Untergeordnete Elemente im Stammverzeichnis des Laufwerk des aktuellen Benutzers auflisten</span><span class="sxs-lookup"><span data-stu-id="2b7fd-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="2b7fd-128">Wenn Sie Dateien aus dem Stammordner des Laufwerks abrufen möchten, wenden Sie die `root`-Beziehung auf das Laufwerk an und greifen Sie dann auf die untergeordnete Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="2b7fd-129">Untergeordnete Elemente eines DriveItem mit einer bekannten ID auflisten</span><span class="sxs-lookup"><span data-stu-id="2b7fd-129">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="2b7fd-130">Wenn Sie Dateien aus dem Stammordner des Laufwerks abrufen möchten, wenden Sie die `root`-Beziehung auf das Laufwerk an und greifen Sie dann auf die untergeordnete Beziehung zu.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="2b7fd-131">Untergeordnete Elemente eines DriveItem mit einem bekannten Pfad auflisten</span><span class="sxs-lookup"><span data-stu-id="2b7fd-131">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="2b7fd-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b7fd-132">Response</span></span>

<span data-ttu-id="2b7fd-133">Wenn die Methode erfolgreich verläuft, wird die Liste der Elemente in der Auflistung der untergeordneten Elemente des Zielelements zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-133">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="2b7fd-134">Die Auflistung untergeordneter Elemente besteht aus [driveItem][item-resource]-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-134">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="2b7fd-135">**Hinweis:** Wenn eine Auflistung die Standardseitengröße (200 Artikel) überschreitet, wird die Eigenschaft **@odata.nextLink** in der Antwort zurückgegeben, damit angezeigt wird, dass mehr Elemente zur Verfügung, und die Anfrage-URL für die nächste Seite von Elementen zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-135">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="2b7fd-136">Sie können die Seitengröße über [Optionale Abfragezeichenfolge-Parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) steuern.</span><span class="sxs-lookup"><span data-stu-id="2b7fd-136">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="2b7fd-137">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="2b7fd-137">Error responses</span></span>

<span data-ttu-id="2b7fd-138">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="2b7fd-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children"
} -->
