# <a name="close-session"></a><span data-ttu-id="a8238-101">Sitzung schließen</span><span class="sxs-lookup"><span data-stu-id="a8238-101">Close Session</span></span>

<span data-ttu-id="a8238-102">Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu schließen.</span><span class="sxs-lookup"><span data-stu-id="a8238-102">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a8238-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8238-103">Permissions</span></span>
<span data-ttu-id="a8238-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8238-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8238-106">Permission type</span></span>      | <span data-ttu-id="a8238-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8238-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8238-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8238-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a8238-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8238-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8238-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8238-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8238-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8238-111">Not supported.</span></span>    |
|<span data-ttu-id="a8238-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8238-112">Application</span></span> | <span data-ttu-id="a8238-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8238-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8238-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8238-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="a8238-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8238-115">Request headers</span></span>
| <span data-ttu-id="a8238-116">Name</span><span class="sxs-lookup"><span data-stu-id="a8238-116">Name</span></span>       | <span data-ttu-id="a8238-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8238-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8238-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8238-118">Authorization</span></span>  | <span data-ttu-id="a8238-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8238-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8238-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a8238-121">Workbook-Session-Id</span></span> | <span data-ttu-id="a8238-122">Arbeitsmappensitzungs-ID zum Schließen</span><span class="sxs-lookup"><span data-stu-id="a8238-122">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8238-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8238-123">Request body</span></span>
<span data-ttu-id="a8238-124">Für diese API ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8238-124">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="a8238-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8238-125">Response</span></span>

<span data-ttu-id="a8238-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8238-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8238-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8238-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8238-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8238-128">Request</span></span>
<span data-ttu-id="a8238-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8238-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="a8238-130">Beachten Sie, dass ein Arbeitsmappesitzungs-ID-Header erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a8238-130">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="a8238-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8238-131">Response</span></span>
<span data-ttu-id="a8238-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8238-132">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```