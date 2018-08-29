# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="0eab1-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="0eab1-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="0eab1-102">Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.</span><span class="sxs-lookup"><span data-stu-id="0eab1-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="0eab1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0eab1-103">Permissions</span></span>
<span data-ttu-id="0eab1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0eab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0eab1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0eab1-106">Permission type</span></span>      | <span data-ttu-id="0eab1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0eab1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eab1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0eab1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0eab1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0eab1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0eab1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0eab1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eab1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0eab1-111">Not supported.</span></span>    |
|<span data-ttu-id="0eab1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0eab1-112">Application</span></span> | <span data-ttu-id="0eab1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0eab1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eab1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eab1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="0eab1-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0eab1-115">Request headers</span></span>
| <span data-ttu-id="0eab1-116">Name</span><span class="sxs-lookup"><span data-stu-id="0eab1-116">Name</span></span>       | <span data-ttu-id="0eab1-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eab1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0eab1-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0eab1-118">Authorization</span></span>  | <span data-ttu-id="0eab1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0eab1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0eab1-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0eab1-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="0eab1-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0eab1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eab1-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0eab1-124">Request body</span></span>
<span data-ttu-id="0eab1-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0eab1-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0eab1-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="0eab1-126">Parameter</span></span>    | <span data-ttu-id="0eab1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0eab1-127">Type</span></span>   |<span data-ttu-id="0eab1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eab1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0eab1-129">color</span><span class="sxs-lookup"><span data-stu-id="0eab1-129">color</span></span>|<span data-ttu-id="0eab1-130">string</span><span class="sxs-lookup"><span data-stu-id="0eab1-130">string</span></span>|<span data-ttu-id="0eab1-131">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="0eab1-131">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="0eab1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eab1-132">Response</span></span>

<span data-ttu-id="0eab1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0eab1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eab1-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0eab1-135">Example</span></span>
<span data-ttu-id="0eab1-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0eab1-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0eab1-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eab1-137">Request</span></span>
<span data-ttu-id="0eab1-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0eab1-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="0eab1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eab1-139">Response</span></span>
<span data-ttu-id="0eab1-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0eab1-140">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->