---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Suchen nach Dateien
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 201102a5332bc6e4ae6fe7d43a71238bb849b21e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481375"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="94cd5-102">Suchen nach DriveItems innerhalb eines Laufwerks</span><span class="sxs-lookup"><span data-stu-id="94cd5-102">Search for a DriveItems within a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94cd5-103">Durchsuchen Sie die Hierarchie der Elemente nach Elementen, die mit einer Abfrage übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="94cd5-103">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="94cd5-104">Sie können innerhalb einer Ordnerhierarchie, eines gesamten Laufwerks oder innerhalb von für den aktuellen Benutzer freigegebenen Dateien suchen.</span><span class="sxs-lookup"><span data-stu-id="94cd5-104">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="94cd5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94cd5-105">Permissions</span></span>

<span data-ttu-id="94cd5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94cd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94cd5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94cd5-108">Permission type</span></span>      | <span data-ttu-id="94cd5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94cd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94cd5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94cd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94cd5-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94cd5-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="94cd5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94cd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94cd5-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94cd5-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="94cd5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94cd5-114">Application</span></span> | <span data-ttu-id="94cd5-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94cd5-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94cd5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94cd5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94cd5-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="94cd5-117">Optional query parameters</span></span>

<span data-ttu-id="94cd5-118">Diese Methode unterstützt die `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94cd5-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="94cd5-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="94cd5-119">Function parameters</span></span>

| <span data-ttu-id="94cd5-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="94cd5-120">Parameter</span></span> | <span data-ttu-id="94cd5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="94cd5-121">Type</span></span>  | <span data-ttu-id="94cd5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94cd5-122">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="94cd5-123">q</span><span class="sxs-lookup"><span data-stu-id="94cd5-123">q</span></span>  | <span data-ttu-id="94cd5-124">string</span><span class="sxs-lookup"><span data-stu-id="94cd5-124">string</span></span> | <span data-ttu-id="94cd5-p103">Der zum Durchsuchen der Elemente verwendete Abfragetext. Werte werden möglicherweise mit mehreren Feldern wie Dateiname, Metadaten und Dateiinhalt abgeglichen.</span><span class="sxs-lookup"><span data-stu-id="94cd5-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="94cd5-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94cd5-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="94cd5-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94cd5-128">Request</span></span>

<span data-ttu-id="94cd5-129">Es folgt ein Beispiel für die Anforderung zum Durchsuchen von OneDrive des aktuellen Benutzers</span><span class="sxs-lookup"><span data-stu-id="94cd5-129">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="94cd5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="94cd5-130">Response</span></span>

<span data-ttu-id="94cd5-p104">Diese Methode gibt ein Objekt mit einer Sammlung von [DriveItems](../resources/driveitem.md)-Elementen zurück, die den Suchkriterien entsprechen. Wenn keine Elemente gefunden werden, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94cd5-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="94cd5-p105">Wenn diese Methode zu viele Ergebnisse zurückgibt, ist die Antwort seitennummeriert und enthält eine **@odata.nextLink**-Eigenschaft mit einer URL zur nächsten Ergebnisseite. Sie können den `$top`-Abfrageparameter zum Angeben der Anzahl der Elemente auf einer Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="94cd5-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="94cd5-135">Suchen nach Elementen, auf die Benutzer zugreifen können</span><span class="sxs-lookup"><span data-stu-id="94cd5-135">Searching for items a user can access</span></span>

<span data-ttu-id="94cd5-p106">Neben Elementen in einem Laufwerk kann Ihre App die Suche auf Elemente erweitern, die für den aktuellen Benutzer freigegeben wurden. Verwenden Sie zum Erweitern des Suchbereichs die **search**-Methode für die [Laufwerk](../resources/drive.md)ressource.</span><span class="sxs-lookup"><span data-stu-id="94cd5-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="94cd5-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94cd5-138">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="94cd5-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="94cd5-139">Response</span></span>

<span data-ttu-id="94cd5-p107">Die Antworten können beim Durchsuchen der **Laufwerk**ressource Elemente enthalten, die sich außerhalb des Laufwerks befinden (Elemente, die für den aktuellen Benutzer freigegeben sind). Diese Elemente enthalten das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass sie außerhalb des Ziellaufwerks gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="94cd5-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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

## <a name="error-responses"></a><span data-ttu-id="94cd5-142">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="94cd5-142">Error responses</span></span>

<span data-ttu-id="94cd5-143">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="94cd5-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-search.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
