# <a name="chartcollection-itemat"></a><span data-ttu-id="1cc62-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="1cc62-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="1cc62-102">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="1cc62-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="1cc62-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1cc62-103">Permissions</span></span>
<span data-ttu-id="1cc62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1cc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1cc62-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1cc62-106">Permission type</span></span>      | <span data-ttu-id="1cc62-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1cc62-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc62-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1cc62-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc62-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cc62-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1cc62-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1cc62-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc62-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1cc62-111">Not supported.</span></span>    |
|<span data-ttu-id="1cc62-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1cc62-112">Application</span></span> | <span data-ttu-id="1cc62-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1cc62-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc62-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1cc62-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="1cc62-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1cc62-115">Request headers</span></span>
| <span data-ttu-id="1cc62-116">Name</span><span class="sxs-lookup"><span data-stu-id="1cc62-116">Name</span></span>       | <span data-ttu-id="1cc62-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cc62-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1cc62-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc62-118">Authorization</span></span>  | <span data-ttu-id="1cc62-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1cc62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc62-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1cc62-121">Request body</span></span>
<span data-ttu-id="1cc62-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1cc62-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1cc62-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="1cc62-123">Parameter</span></span>    | <span data-ttu-id="1cc62-124">Typ</span><span class="sxs-lookup"><span data-stu-id="1cc62-124">Type</span></span>   |<span data-ttu-id="1cc62-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cc62-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc62-126">Index</span><span class="sxs-lookup"><span data-stu-id="1cc62-126">index</span></span>|<span data-ttu-id="1cc62-127">number</span><span class="sxs-lookup"><span data-stu-id="1cc62-127">number</span></span>|<span data-ttu-id="1cc62-p103">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="1cc62-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1cc62-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1cc62-130">Response</span></span>

<span data-ttu-id="1cc62-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1cc62-131">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cc62-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1cc62-132">Example</span></span>
<span data-ttu-id="1cc62-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1cc62-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1cc62-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1cc62-134">Request</span></span>
<span data-ttu-id="1cc62-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1cc62-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="1cc62-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1cc62-136">Response</span></span>
<span data-ttu-id="1cc62-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1cc62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->