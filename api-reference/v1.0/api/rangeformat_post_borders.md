# <a name="create-rangeborder"></a><span data-ttu-id="a48e0-101">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="a48e0-101">Create RangeBorder</span></span>

<span data-ttu-id="a48e0-102">Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="a48e0-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a48e0-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a48e0-103">Permissions</span></span>
<span data-ttu-id="a48e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a48e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a48e0-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a48e0-106">Permission type</span></span>      | <span data-ttu-id="a48e0-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a48e0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a48e0-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a48e0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a48e0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a48e0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a48e0-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a48e0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a48e0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a48e0-111">Not supported.</span></span>    |
|<span data-ttu-id="a48e0-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a48e0-112">Application</span></span> | <span data-ttu-id="a48e0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a48e0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a48e0-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a48e0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="a48e0-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a48e0-115">Request headers</span></span>
| <span data-ttu-id="a48e0-116">Name</span><span class="sxs-lookup"><span data-stu-id="a48e0-116">Name</span></span>       | <span data-ttu-id="a48e0-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a48e0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a48e0-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a48e0-118">Authorization</span></span>  | <span data-ttu-id="a48e0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a48e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a48e0-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a48e0-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a48e0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a48e0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a48e0-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a48e0-124">Request body</span></span>
<span data-ttu-id="a48e0-125">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookRangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a48e0-125">In the request body, supply a JSON representation of [directoryObject](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a48e0-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="a48e0-126">Response</span></span>

<span data-ttu-id="a48e0-127">Wenn erfolgreich, gibt diese Methode einen Antwortcode `201 Created` und das [WorkbookRangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a48e0-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a48e0-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a48e0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a48e0-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a48e0-129">Request</span></span>
<span data-ttu-id="a48e0-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a48e0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="a48e0-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookRangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a48e0-131">In the request body, supply a JSON representation of [plannerPlan](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a48e0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a48e0-132">Response</span></span>
<span data-ttu-id="a48e0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a48e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->