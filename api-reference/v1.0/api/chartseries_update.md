# <a name="update-chartseries"></a><span data-ttu-id="a51d2-101">ChartSeries aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a51d2-101">Update chartseries</span></span>

<span data-ttu-id="a51d2-102">Dient zum Aktualisieren der Eigenschaften des ChartSeries-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a51d2-102">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a51d2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a51d2-103">Permissions</span></span>
<span data-ttu-id="a51d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a51d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a51d2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a51d2-106">Permission type</span></span>      | <span data-ttu-id="a51d2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a51d2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a51d2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a51d2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a51d2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a51d2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a51d2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a51d2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a51d2-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a51d2-111">Not supported.</span></span>    |
|<span data-ttu-id="a51d2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a51d2-112">Application</span></span> | <span data-ttu-id="a51d2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a51d2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a51d2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a51d2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a51d2-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a51d2-115">Optional request headers</span></span>
| <span data-ttu-id="a51d2-116">Name</span><span class="sxs-lookup"><span data-stu-id="a51d2-116">Name</span></span>       | <span data-ttu-id="a51d2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a51d2-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a51d2-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a51d2-118">Authorization</span></span>  | <span data-ttu-id="a51d2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a51d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a51d2-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a51d2-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a51d2-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a51d2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a51d2-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a51d2-124">Request body</span></span>
<span data-ttu-id="a51d2-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a51d2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a51d2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a51d2-128">Property</span></span>     | <span data-ttu-id="a51d2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a51d2-129">Type</span></span>   |<span data-ttu-id="a51d2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a51d2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a51d2-131">Name</span><span class="sxs-lookup"><span data-stu-id="a51d2-131">name</span></span>|<span data-ttu-id="a51d2-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a51d2-132">string</span></span>|<span data-ttu-id="a51d2-133">Gibt den Namen einer Datenreihe in einem Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="a51d2-133">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="a51d2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a51d2-134">Response</span></span>

<span data-ttu-id="a51d2-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [WorkbookChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a51d2-135">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a51d2-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a51d2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a51d2-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a51d2-137">Request</span></span>
<span data-ttu-id="a51d2-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a51d2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="a51d2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a51d2-139">Response</span></span>
<span data-ttu-id="a51d2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a51d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->