---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Nach Dateien suchen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ee1d8f6ba1c22426beb70d9ad89650e48e6900ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959692"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="ac05b-102">Suchen nach DriveItems innerhalb eines Laufwerks</span><span class="sxs-lookup"><span data-stu-id="ac05b-102">Search for a DriveItems within a drive</span></span>

> <span data-ttu-id="ac05b-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac05b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac05b-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac05b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac05b-105">Durchsuchen Sie die Hierarchie der Elemente nach Elementen, die mit einer Abfrage übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="ac05b-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="ac05b-106">Sie können innerhalb einer Ordnerhierarchie, eines gesamten Laufwerks oder innerhalb von für den aktuellen Benutzer freigegebenen Dateien suchen.</span><span class="sxs-lookup"><span data-stu-id="ac05b-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac05b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ac05b-107">Permissions</span></span>

<span data-ttu-id="ac05b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac05b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac05b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac05b-110">Permission type</span></span>      | <span data-ttu-id="ac05b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac05b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac05b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac05b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac05b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac05b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac05b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac05b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac05b-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac05b-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac05b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac05b-116">Application</span></span> | <span data-ttu-id="ac05b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac05b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac05b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac05b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac05b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ac05b-119">Optional query parameters</span></span>

<span data-ttu-id="ac05b-120">Diese Methode unterstützt die `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac05b-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="ac05b-121">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="ac05b-121">Function parameters</span></span>

| <span data-ttu-id="ac05b-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="ac05b-122">Parameter</span></span> | <span data-ttu-id="ac05b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ac05b-123">Type</span></span>  | <span data-ttu-id="ac05b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac05b-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ac05b-125">q</span><span class="sxs-lookup"><span data-stu-id="ac05b-125">q</span></span>  | <span data-ttu-id="ac05b-126">string</span><span class="sxs-lookup"><span data-stu-id="ac05b-126">string</span></span> | <span data-ttu-id="ac05b-p104">Der zum Durchsuchen der Elemente verwendete Abfragetext. Werte werden möglicherweise mit mehreren Feldern wie Dateiname, Metadaten und Dateiinhalt abgeglichen.</span><span class="sxs-lookup"><span data-stu-id="ac05b-p104">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="ac05b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac05b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac05b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac05b-130">Request</span></span>

<span data-ttu-id="ac05b-131">Es folgt ein Beispiel für die Anforderung zum Durchsuchen von OneDrive des aktuellen Benutzers</span><span class="sxs-lookup"><span data-stu-id="ac05b-131">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="ac05b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac05b-132">Response</span></span>

<span data-ttu-id="ac05b-p105">Diese Methode gibt ein Objekt mit einer Sammlung von [DriveItems](../resources/driveitem.md)-Elementen zurück, die den Suchkriterien entsprechen. Wenn keine Elemente gefunden werden, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac05b-p105">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="ac05b-p106">Wenn diese Methode zu viele Ergebnisse zurückgibt, ist die Antwort seitennummeriert und enthält eine **@odata.nextLink**-Eigenschaft mit einer URL zur nächsten Ergebnisseite. Sie können den `$top`-Abfrageparameter zum Angeben der Anzahl der Elemente auf einer Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="ac05b-p106">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="ac05b-137">Suchen nach Elementen, auf die Benutzer zugreifen können</span><span class="sxs-lookup"><span data-stu-id="ac05b-137">Searching for items a user can access</span></span>

<span data-ttu-id="ac05b-p107">Neben Elementen in einem Laufwerk kann Ihre App die Suche auf Elemente erweitern, die für den aktuellen Benutzer freigegeben wurden. Verwenden Sie zum Erweitern des Suchbereichs die **search**-Methode für die [Laufwerk](../resources/drive.md)ressource.</span><span class="sxs-lookup"><span data-stu-id="ac05b-p107">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="ac05b-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac05b-140">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="ac05b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac05b-141">Response</span></span>

<span data-ttu-id="ac05b-p108">Die Antworten können beim Durchsuchen der **Laufwerk**ressource Elemente enthalten, die sich außerhalb des Laufwerks befinden (Elemente, die für den aktuellen Benutzer freigegeben sind). Diese Elemente enthalten das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass sie außerhalb des Ziellaufwerks gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="ac05b-p108">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="ac05b-144">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="ac05b-144">Error responses</span></span>

<span data-ttu-id="ac05b-145">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="ac05b-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search"
} -->
