# <a name="create-chartseries"></a><span data-ttu-id="12365-101">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="12365-101">Create ChartSeries</span></span>

<span data-ttu-id="12365-102">Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="12365-102">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="12365-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12365-103">Permissions</span></span>
<span data-ttu-id="12365-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12365-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12365-106">Permission type</span></span>      | <span data-ttu-id="12365-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12365-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12365-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12365-108">Delegated (work or school account)</span></span> | <span data-ttu-id="12365-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12365-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12365-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12365-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12365-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12365-111">Not supported.</span></span>    |
|<span data-ttu-id="12365-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12365-112">Application</span></span> | <span data-ttu-id="12365-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12365-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12365-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12365-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="12365-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12365-115">Request headers</span></span>
| <span data-ttu-id="12365-116">Name</span><span class="sxs-lookup"><span data-stu-id="12365-116">Name</span></span>       | <span data-ttu-id="12365-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12365-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12365-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="12365-118">Authorization</span></span>  | <span data-ttu-id="12365-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12365-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12365-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="12365-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="12365-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="12365-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12365-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12365-124">Request body</span></span>
<span data-ttu-id="12365-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="12365-125">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12365-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="12365-126">Response</span></span>

<span data-ttu-id="12365-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12365-127">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12365-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12365-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12365-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12365-129">Request</span></span>
<span data-ttu-id="12365-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12365-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="12365-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="12365-131">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12365-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="12365-132">Response</span></span>
<span data-ttu-id="12365-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12365-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->