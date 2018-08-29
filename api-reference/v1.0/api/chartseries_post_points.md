# <a name="create-chartpoints"></a><span data-ttu-id="cf003-101">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="cf003-101">Create ChartPoints</span></span>

<span data-ttu-id="cf003-102">Verwenden Sie diese API, um neue ChartPoints zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="cf003-102">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf003-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf003-103">Permissions</span></span>
<span data-ttu-id="cf003-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf003-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf003-106">Permission type</span></span>      | <span data-ttu-id="cf003-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf003-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf003-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf003-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cf003-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf003-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf003-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf003-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf003-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf003-111">Not supported.</span></span>    |
|<span data-ttu-id="cf003-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf003-112">Application</span></span> | <span data-ttu-id="cf003-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf003-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf003-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf003-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points

```
## <a name="request-headers"></a><span data-ttu-id="cf003-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf003-115">Request headers</span></span>
| <span data-ttu-id="cf003-116">Name</span><span class="sxs-lookup"><span data-stu-id="cf003-116">Name</span></span>       | <span data-ttu-id="cf003-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf003-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf003-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cf003-118">Authorization</span></span>  | <span data-ttu-id="cf003-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf003-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf003-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cf003-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="cf003-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cf003-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf003-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf003-124">Request body</span></span>
<span data-ttu-id="cf003-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cf003-125">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf003-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf003-126">Response</span></span>

<span data-ttu-id="cf003-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ChartPoints](../resources/chartpoint.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf003-127">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf003-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf003-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf003-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf003-129">Request</span></span>
<span data-ttu-id="cf003-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf003-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="cf003-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cf003-131">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cf003-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf003-132">Response</span></span>
<span data-ttu-id="cf003-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf003-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->