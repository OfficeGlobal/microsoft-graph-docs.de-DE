# <a name="create-chartseries"></a><span data-ttu-id="4d759-101">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="4d759-101">Create ChartSeries</span></span>

<span data-ttu-id="4d759-102">Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d759-102">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d759-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d759-103">Permissions</span></span>
<span data-ttu-id="4d759-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d759-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d759-106">Permission type</span></span>      | <span data-ttu-id="4d759-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d759-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d759-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d759-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4d759-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d759-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d759-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d759-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d759-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d759-111">Not supported.</span></span>    |
|<span data-ttu-id="4d759-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d759-112">Application</span></span> | <span data-ttu-id="4d759-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d759-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d759-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d759-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="4d759-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d759-115">Request headers</span></span>
| <span data-ttu-id="4d759-116">Name</span><span class="sxs-lookup"><span data-stu-id="4d759-116">Name</span></span>       | <span data-ttu-id="4d759-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d759-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d759-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d759-118">Authorization</span></span>  | <span data-ttu-id="4d759-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d759-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d759-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d759-121">Request body</span></span>
<span data-ttu-id="4d759-122">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d759-122">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d759-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d759-123">Response</span></span>

<span data-ttu-id="4d759-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d759-124">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d759-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d759-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d759-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d759-126">Request</span></span>
<span data-ttu-id="4d759-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d759-127">Here is an example of the request.</span></span>
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
<span data-ttu-id="4d759-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d759-128">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4d759-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d759-129">Response</span></span>
<span data-ttu-id="4d759-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d759-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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