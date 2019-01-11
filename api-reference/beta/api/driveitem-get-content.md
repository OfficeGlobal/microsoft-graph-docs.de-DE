---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei herunterladen
localization_priority: Normal
ms.openlocfilehash: ac391f5ffb6af9fc288bdc22cf0dbf3c77dca0b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854754"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="8a4e8-102">Inhalte von DriveItem herunterladen</span><span class="sxs-lookup"><span data-stu-id="8a4e8-102">Download the contents of a DriveItem</span></span>

> <span data-ttu-id="8a4e8-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a4e8-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a4e8-105">Laden Sie die Inhalte des primären Streams (Datei) eines DriveItem herunter.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-105">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="8a4e8-106">Es können nur driveItems mit der Eigenschaft **file** heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-106">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a4e8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a4e8-107">Permissions</span></span>

<span data-ttu-id="8a4e8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a4e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a4e8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a4e8-110">Permission type</span></span>      | <span data-ttu-id="8a4e8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a4e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a4e8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a4e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4e8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4e8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a4e8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a4e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4e8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4e8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a4e8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a4e8-116">Application</span></span> | <span data-ttu-id="8a4e8-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a4e8-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a4e8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a4e8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="8a4e8-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a4e8-119">Optional request headers</span></span>

| <span data-ttu-id="8a4e8-120">Name</span><span class="sxs-lookup"><span data-stu-id="8a4e8-120">Name</span></span>          | <span data-ttu-id="8a4e8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8a4e8-121">Value</span></span>  | <span data-ttu-id="8a4e8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a4e8-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8a4e8-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="8a4e8-123">if-none-match</span></span> | <span data-ttu-id="8a4e8-124">String</span><span class="sxs-lookup"><span data-stu-id="8a4e8-124">String</span></span> | <span data-ttu-id="8a4e8-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="8a4e8-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a4e8-126">Example</span></span>

<span data-ttu-id="8a4e8-127">Dies ist ein Beispiel für das Herunterladen einer vollständigen Datei.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-127">Here is an example to download a complete file.</span></span>


<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```

### <a name="response"></a><span data-ttu-id="8a4e8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a4e8-128">Response</span></span>

<span data-ttu-id="8a4e8-p104">Gibt eine `302 Found`-Antwort zurück, mit der zu einer zuvor authentifizierten Download-URL umgeleitet wird. Dies ist dieselbe URL, die `@microsoft.graph.downloadUrl`-Eigenschaft für DriveItem verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="8a4e8-p105">Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-p105">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="8a4e8-133">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-133">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="8a4e8-134">Teilbereichdownloads</span><span class="sxs-lookup"><span data-stu-id="8a4e8-134">Partial range downloads</span></span>

<span data-ttu-id="8a4e8-p106">Zum Herunterladen eines Teilbereichs von Bytes aus einer Datei kann die App den `Range`-Header gemäß der Angabe in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) verwenden. Sie müssen den `Range`-Header an die tatsächliche `@microsoft.graph.downloadUrl`-URL anfügen, und nicht an die Anforderung für `/content`.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="8a4e8-p107">Es wird eine `HTTP 206 Partial Content`-Antwort mit dem Anforderungsbereich von Bytes aus der Datei zurückgegeben. Wenn der Bereich nicht generiert werden kann, wird der Range-Header möglicherweise ignoriert und gibt eine `HTTP 200`-Antwort mit dem gesamten Inhalt der Datei zurück.</span><span class="sxs-lookup"><span data-stu-id="8a4e8-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="8a4e8-139">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="8a4e8-139">Error responses</span></span>

<span data-ttu-id="8a4e8-140">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="8a4e8-140">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download"
} -->
