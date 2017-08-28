# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="4b955-101">Inhalte von DriveItem herunterladen</span><span class="sxs-lookup"><span data-stu-id="4b955-101">Download the contents of a DriveItem</span></span>

<span data-ttu-id="4b955-p101">Laden Sie die Inhalte für driveItem herunter. Es können nur driveItem-Elemente mit der **file**-Eigenschaft heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="4b955-p101">Download the contents for a driveItem. Only driveItem with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b955-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b955-104">Permissions</span></span>
<span data-ttu-id="4b955-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b955-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b955-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b955-107">Permission type</span></span>      | <span data-ttu-id="4b955-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b955-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b955-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b955-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4b955-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b955-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b955-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b955-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b955-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b955-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b955-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b955-113">Application</span></span> | <span data-ttu-id="4b955-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b955-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b955-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b955-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /drives/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
```

## <a name="request-headers"></a><span data-ttu-id="4b955-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b955-116">Request headers</span></span>

| <span data-ttu-id="4b955-117">Name</span><span class="sxs-lookup"><span data-stu-id="4b955-117">Name</span></span>          | <span data-ttu-id="4b955-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4b955-118">Value</span></span>  | <span data-ttu-id="4b955-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b955-119">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b955-120">if-none-match</span><span class="sxs-lookup"><span data-stu-id="4b955-120">if-none-match</span></span> | <span data-ttu-id="4b955-121">String</span><span class="sxs-lookup"><span data-stu-id="4b955-121">String</span></span> | <span data-ttu-id="4b955-122">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b955-122">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b955-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b955-123">Request body</span></span>
<span data-ttu-id="4b955-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4b955-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="4b955-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b955-125">Example</span></span>
<span data-ttu-id="4b955-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4b955-126">Here is an example of how to call this API.</span></span>


<!-- { "blockType": "request", "name": "driveitem-download-contents" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/content
```

##### <a name="response"></a><span data-ttu-id="4b955-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b955-127">Response</span></span>
<span data-ttu-id="4b955-p103">Gibt eine `302 Found`-Antwort zurück, mit der zu einer zuvor authentifizierten Download-URL umgeleitet wird. Dies ist dieselbe URL, die `@microsoft.graph.downloadUrl`-Eigenschaft für DriveItem verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="4b955-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="4b955-p104">Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.</span><span class="sxs-lookup"><span data-stu-id="4b955-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="4b955-132">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="4b955-132">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="4b955-133">Teilbereichdownloads</span><span class="sxs-lookup"><span data-stu-id="4b955-133">Partial range downloads</span></span>

<span data-ttu-id="4b955-p105">Zum Herunterladen eines Teilbereichs von Bytes aus einer Datei kann die App den `Range`-Header gemäß der Angabe in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) verwenden. Sie müssen den `Range`-Header an die tatsächliche `@microsoft.graph.downloadUrl`-URL anfügen, und nicht an die Anforderung für `/content`.</span><span class="sxs-lookup"><span data-stu-id="4b955-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "driveitem-get-partial-content" } -->
```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="4b955-p106">Es wird eine `HTTP 206 Partial Content`-Antwort mit dem Anforderungsbereich von Bytes aus der Datei zurückgegeben. Wenn der Bereich nicht generiert werden kann, wird der Range-Header möglicherweise ignoriert und gibt eine `HTTP 200`-Antwort mit dem gesamten Inhalt der Datei zurück.</span><span class="sxs-lookup"><span data-stu-id="4b955-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Download item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Download file"
}-->
