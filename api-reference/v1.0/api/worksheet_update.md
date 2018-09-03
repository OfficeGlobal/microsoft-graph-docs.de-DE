# <a name="update-worksheet"></a><span data-ttu-id="e99f4-101">Arbeitsblatt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e99f4-101">Update worksheet</span></span>

<span data-ttu-id="e99f4-102">Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.</span><span class="sxs-lookup"><span data-stu-id="e99f4-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e99f4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e99f4-103">Permissions</span></span>
<span data-ttu-id="e99f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e99f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e99f4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e99f4-106">Permission type</span></span>      | <span data-ttu-id="e99f4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e99f4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e99f4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e99f4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e99f4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e99f4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e99f4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e99f4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99f4-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e99f4-111">Not supported.</span></span>    |
|<span data-ttu-id="e99f4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e99f4-112">Application</span></span> | <span data-ttu-id="e99f4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e99f4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e99f4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99f4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e99f4-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e99f4-115">Optional request headers</span></span>
| <span data-ttu-id="e99f4-116">Name</span><span class="sxs-lookup"><span data-stu-id="e99f4-116">Name</span></span>       | <span data-ttu-id="e99f4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e99f4-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e99f4-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e99f4-118">Authorization</span></span>  | <span data-ttu-id="e99f4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e99f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e99f4-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e99f4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e99f4-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e99f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e99f4-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e99f4-124">Request body</span></span>
<span data-ttu-id="e99f4-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e99f4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e99f4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e99f4-128">Property</span></span>     | <span data-ttu-id="e99f4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e99f4-129">Type</span></span>   |<span data-ttu-id="e99f4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e99f4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e99f4-131">Name</span><span class="sxs-lookup"><span data-stu-id="e99f4-131">name</span></span>|<span data-ttu-id="e99f4-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e99f4-132">string</span></span>|<span data-ttu-id="e99f4-133">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="e99f4-133">The display name of the worksheet.</span></span>|
|<span data-ttu-id="e99f4-134">position</span><span class="sxs-lookup"><span data-stu-id="e99f4-134">position</span></span>|<span data-ttu-id="e99f4-135">int</span><span class="sxs-lookup"><span data-stu-id="e99f4-135">int</span></span>|<span data-ttu-id="e99f4-136">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="e99f4-136">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="e99f4-137">visibility</span><span class="sxs-lookup"><span data-stu-id="e99f4-137">visibility</span></span>|<span data-ttu-id="e99f4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e99f4-138">string</span></span>|<span data-ttu-id="e99f4-139">Die Sichtbarkeit des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="e99f4-139">The Visibility of the worksheet. Possible values are: , , .</span></span> <span data-ttu-id="e99f4-140">Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="e99f4-140">The possible values are `Visible`, `Hidden`, `VeryHidden`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="e99f4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99f4-141">Response</span></span>

<span data-ttu-id="e99f4-142">Wenn erfolgreich, gibt dieses Verfahren im Antworttext einen `200 OK` Antwortcode und ein[WorkbookWorksheet](../resources/worksheet.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="e99f4-142">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e99f4-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e99f4-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e99f4-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e99f4-144">Request</span></span>
<span data-ttu-id="e99f4-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e99f4-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="e99f4-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="e99f4-146">Response</span></span>
<span data-ttu-id="e99f4-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e99f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->