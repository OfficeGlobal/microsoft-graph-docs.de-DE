# <a name="chartfill-clear"></a><span data-ttu-id="4a048-101">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="4a048-101">ChartFill: clear</span></span>

<span data-ttu-id="4a048-102">Dient zum Löschen der Füllfarbe eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="4a048-102">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a048-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a048-103">Permissions</span></span>
<span data-ttu-id="4a048-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a048-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a048-106">Permission type</span></span>      | <span data-ttu-id="4a048-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a048-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a048-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a048-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a048-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a048-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a048-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a048-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a048-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a048-111">Not supported.</span></span>    |
|<span data-ttu-id="4a048-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a048-112">Application</span></span> | <span data-ttu-id="4a048-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a048-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a048-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a048-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="4a048-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a048-115">Request headers</span></span>
| <span data-ttu-id="4a048-116">Name</span><span class="sxs-lookup"><span data-stu-id="4a048-116">Name</span></span>       | <span data-ttu-id="4a048-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a048-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a048-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4a048-118">Authorization</span></span>  | <span data-ttu-id="4a048-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a048-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a048-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4a048-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a048-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4a048-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a048-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a048-124">Request body</span></span>
<span data-ttu-id="4a048-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a048-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a048-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a048-126">Response</span></span>

<span data-ttu-id="4a048-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a048-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a048-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a048-129">Example</span></span>
<span data-ttu-id="4a048-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a048-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a048-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a048-131">Request</span></span>
<span data-ttu-id="4a048-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a048-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="4a048-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a048-133">Response</span></span>
<span data-ttu-id="4a048-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a048-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->