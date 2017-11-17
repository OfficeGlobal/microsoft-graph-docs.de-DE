# <a name="chart-setdata"></a><span data-ttu-id="bf3b3-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="bf3b3-101">Chart: setData</span></span>

<span data-ttu-id="bf3b3-102">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf3b3-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bf3b3-103">Permissions</span></span>
<span data-ttu-id="bf3b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf3b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf3b3-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf3b3-106">Permission type</span></span>      | <span data-ttu-id="bf3b3-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf3b3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf3b3-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf3b3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bf3b3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf3b3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf3b3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf3b3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf3b3-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf3b3-111">Not supported.</span></span>    |
|<span data-ttu-id="bf3b3-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf3b3-112">Application</span></span> | <span data-ttu-id="bf3b3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf3b3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf3b3-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf3b3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="bf3b3-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf3b3-115">Request headers</span></span>
| <span data-ttu-id="bf3b3-116">Name</span><span class="sxs-lookup"><span data-stu-id="bf3b3-116">Name</span></span>       | <span data-ttu-id="bf3b3-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf3b3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf3b3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf3b3-118">Authorization</span></span>  | <span data-ttu-id="bf3b3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf3b3-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf3b3-121">Request body</span></span>
<span data-ttu-id="bf3b3-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf3b3-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="bf3b3-123">Parameter</span></span>    | <span data-ttu-id="bf3b3-124">Typ</span><span class="sxs-lookup"><span data-stu-id="bf3b3-124">Type</span></span>   |<span data-ttu-id="bf3b3-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf3b3-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf3b3-126">sourceData</span><span class="sxs-lookup"><span data-stu-id="bf3b3-126">sourceData</span></span>|<span data-ttu-id="bf3b3-127">string</span><span class="sxs-lookup"><span data-stu-id="bf3b3-127">string</span></span>|<span data-ttu-id="bf3b3-128">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-128">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="bf3b3-129">seriesBy</span><span class="sxs-lookup"><span data-stu-id="bf3b3-129">seriesBy</span></span>|<span data-ttu-id="bf3b3-130">string</span><span class="sxs-lookup"><span data-stu-id="bf3b3-130">string</span></span>|<span data-ttu-id="bf3b3-p103">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden. Folgende Ergebnisse sind möglich: Auto (Standard), Rows, Columns.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-p103">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="bf3b3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf3b3-135">Response</span></span>

<span data-ttu-id="bf3b3-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf3b3-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf3b3-138">Example</span></span>
<span data-ttu-id="bf3b3-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf3b3-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf3b3-140">Request</span></span>
<span data-ttu-id="bf3b3-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="bf3b3-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf3b3-142">Response</span></span>
<span data-ttu-id="bf3b3-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->