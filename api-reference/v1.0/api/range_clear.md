# <a name="range-clear"></a><span data-ttu-id="68822-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="68822-101">Range: clear</span></span>

<span data-ttu-id="68822-102">Löschen von Bereichswerten, Format, Füllung, Rahmen usw.</span><span class="sxs-lookup"><span data-stu-id="68822-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="68822-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68822-103">Permissions</span></span>
<span data-ttu-id="68822-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68822-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68822-106">Permission type</span></span>      | <span data-ttu-id="68822-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68822-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68822-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68822-108">Delegated (work or school account)</span></span> | <span data-ttu-id="68822-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68822-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="68822-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68822-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68822-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68822-111">Not supported.</span></span>    |
|<span data-ttu-id="68822-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68822-112">Application</span></span> | <span data-ttu-id="68822-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68822-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68822-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68822-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="68822-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68822-115">Request headers</span></span>
| <span data-ttu-id="68822-116">Name</span><span class="sxs-lookup"><span data-stu-id="68822-116">Name</span></span>       | <span data-ttu-id="68822-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68822-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="68822-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="68822-118">Authorization</span></span>  | <span data-ttu-id="68822-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68822-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68822-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="68822-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="68822-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="68822-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68822-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68822-124">Request body</span></span>
<span data-ttu-id="68822-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="68822-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68822-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="68822-126">Parameter</span></span>    | <span data-ttu-id="68822-127">Typ</span><span class="sxs-lookup"><span data-stu-id="68822-127">Type</span></span>   |<span data-ttu-id="68822-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68822-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68822-129">applyTo</span><span class="sxs-lookup"><span data-stu-id="68822-129">applyTo</span></span>|<span data-ttu-id="68822-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68822-130">string</span></span>|<span data-ttu-id="68822-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="68822-131">Optional.</span></span> <span data-ttu-id="68822-132">Bestimmt den Typ der Aktion deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="68822-132">Optional. Determines the type of clear action.  Possible values are: , , .</span></span>  <span data-ttu-id="68822-133">Die möglichen Werte sind: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="68822-133">The possible values are `All`, `Formats`, `Contents`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="68822-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="68822-134">Response</span></span>

<span data-ttu-id="68822-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68822-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68822-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68822-137">Example</span></span>
<span data-ttu-id="68822-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="68822-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="68822-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68822-139">Request</span></span>
<span data-ttu-id="68822-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68822-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="68822-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="68822-141">Response</span></span>
<span data-ttu-id="68822-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68822-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->