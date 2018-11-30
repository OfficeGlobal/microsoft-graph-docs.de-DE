---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei herunterladen
ms.openlocfilehash: 0c6f509c6b204789b14899fcafe8763f713511d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018458"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="e45c6-102">Inhalte von DriveItem herunterladen</span><span class="sxs-lookup"><span data-stu-id="e45c6-102">Download the contents of a DriveItem</span></span>

<span data-ttu-id="e45c6-103">Laden Sie die Inhalte des primären Streams (Datei) eines DriveItem herunter.</span><span class="sxs-lookup"><span data-stu-id="e45c6-103">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="e45c6-104">Es können nur driveItems mit der Eigenschaft **file** heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="e45c6-104">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="e45c6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e45c6-105">Permissions</span></span>

<span data-ttu-id="e45c6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45c6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e45c6-108">Permission type</span></span>      | <span data-ttu-id="e45c6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e45c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e45c6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e45c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e45c6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45c6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e45c6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e45c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e45c6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45c6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e45c6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e45c6-114">Application</span></span> | <span data-ttu-id="e45c6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45c6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e45c6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e45c6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="e45c6-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e45c6-117">Optional request headers</span></span>

| <span data-ttu-id="e45c6-118">Name</span><span class="sxs-lookup"><span data-stu-id="e45c6-118">Name</span></span>          | <span data-ttu-id="e45c6-119">Wert</span><span class="sxs-lookup"><span data-stu-id="e45c6-119">Value</span></span>  | <span data-ttu-id="e45c6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e45c6-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e45c6-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="e45c6-121">if-none-match</span></span> | <span data-ttu-id="e45c6-122">String</span><span class="sxs-lookup"><span data-stu-id="e45c6-122">String</span></span> | <span data-ttu-id="e45c6-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e45c6-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="e45c6-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e45c6-124">Example</span></span>

<span data-ttu-id="e45c6-125">Dies ist ein Beispiel für das Herunterladen einer vollständigen Datei.</span><span class="sxs-lookup"><span data-stu-id="e45c6-125">Here is an example to download a complete file.</span></span>


<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```

### <a name="response"></a><span data-ttu-id="e45c6-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e45c6-126">Response</span></span>

<span data-ttu-id="e45c6-p103">Gibt eine `302 Found`-Antwort zurück, mit der zu einer zuvor authentifizierten Download-URL umgeleitet wird. Dies ist dieselbe URL, die `@microsoft.graph.downloadUrl`-Eigenschaft für DriveItem verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="e45c6-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="e45c6-129">Zum Herunterladen des Dateiinhalts muss die Anwendung den `Location`-Header in der Antwort aufrufen.</span><span class="sxs-lookup"><span data-stu-id="e45c6-129">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="e45c6-130">Viele HTTP-Client-Bibliotheken werden automatisch die 302-Umleitung und beginnt mit dem Herunterladen der Datei unmittelbar folgen.</span><span class="sxs-lookup"><span data-stu-id="e45c6-130">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="e45c6-131">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="e45c6-131">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="e45c6-132">Teilbereichdownloads</span><span class="sxs-lookup"><span data-stu-id="e45c6-132">Partial range downloads</span></span>

<span data-ttu-id="e45c6-p105">Zum Herunterladen eines Teilbereichs von Bytes aus einer Datei kann die App den `Range`-Header gemäß der Angabe in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) verwenden. Sie müssen den `Range`-Header an die tatsächliche `@microsoft.graph.downloadUrl`-URL anfügen, und nicht an die Anforderung für `/content`.</span><span class="sxs-lookup"><span data-stu-id="e45c6-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="e45c6-p106">Es wird eine `HTTP 206 Partial Content`-Antwort mit dem Anforderungsbereich von Bytes aus der Datei zurückgegeben. Wenn der Bereich nicht generiert werden kann, wird der Range-Header möglicherweise ignoriert und gibt eine `HTTP 200`-Antwort mit dem gesamten Inhalt der Datei zurück.</span><span class="sxs-lookup"><span data-stu-id="e45c6-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="e45c6-137">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="e45c6-137">Error responses</span></span>

<span data-ttu-id="e45c6-138">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="e45c6-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download"
} -->