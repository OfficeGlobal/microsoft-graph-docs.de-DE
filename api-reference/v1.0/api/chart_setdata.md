# <a name="chart-setdata"></a><span data-ttu-id="eb477-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="eb477-101">Chart: setData</span></span>

<span data-ttu-id="eb477-102">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="eb477-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb477-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb477-103">Permissions</span></span>
<span data-ttu-id="eb477-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb477-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb477-106">Permission type</span></span>      | <span data-ttu-id="eb477-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb477-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb477-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb477-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eb477-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb477-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb477-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb477-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb477-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb477-111">Not supported.</span></span>    |
|<span data-ttu-id="eb477-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb477-112">Application</span></span> | <span data-ttu-id="eb477-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb477-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb477-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb477-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="eb477-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb477-115">Request headers</span></span>
| <span data-ttu-id="eb477-116">Name</span><span class="sxs-lookup"><span data-stu-id="eb477-116">Name</span></span>       | <span data-ttu-id="eb477-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb477-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb477-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eb477-118">Authorization</span></span>  | <span data-ttu-id="eb477-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb477-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb477-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="eb477-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb477-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="eb477-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb477-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb477-124">Request body</span></span>
<span data-ttu-id="eb477-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="eb477-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb477-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="eb477-126">Parameter</span></span>    | <span data-ttu-id="eb477-127">Typ</span><span class="sxs-lookup"><span data-stu-id="eb477-127">Type</span></span>   |<span data-ttu-id="eb477-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb477-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb477-129">sourceData</span><span class="sxs-lookup"><span data-stu-id="eb477-129">sourceData</span></span>|<span data-ttu-id="eb477-130">Json</span><span class="sxs-lookup"><span data-stu-id="eb477-130">Json</span></span>|<span data-ttu-id="eb477-131">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="eb477-131">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="eb477-132">seriesBy</span><span class="sxs-lookup"><span data-stu-id="eb477-132">seriesBy</span></span>|<span data-ttu-id="eb477-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb477-133">string</span></span>|<span data-ttu-id="eb477-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="eb477-134">Optional.</span></span> <span data-ttu-id="eb477-135">Gibt an, wie die Spalten und Zeilen als Datenreihen im Diagramm verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="eb477-135">Returns or sets the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="eb477-136">Kann eine der folgenden sein: Automatisch (Standard), Zeilen, Spalten.</span><span class="sxs-lookup"><span data-stu-id="eb477-136">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="eb477-137">Die möglichen Werte sind `Auto`, `Columns`,`Rows`.</span><span class="sxs-lookup"><span data-stu-id="eb477-137">The possible values are `Auto`, `Columns`, `Rows`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="eb477-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb477-138">Response</span></span>

<span data-ttu-id="eb477-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb477-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb477-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb477-141">Example</span></span>
<span data-ttu-id="eb477-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="eb477-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb477-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb477-143">Request</span></span>
<span data-ttu-id="eb477-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb477-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="eb477-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb477-145">Response</span></span>
<span data-ttu-id="eb477-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb477-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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