# <a name="update-worksheet"></a><span data-ttu-id="81a76-101">Arbeitsblatt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="81a76-101">Update worksheet</span></span>

<span data-ttu-id="81a76-102">Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.</span><span class="sxs-lookup"><span data-stu-id="81a76-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="81a76-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="81a76-103">Permissions</span></span>
<span data-ttu-id="81a76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81a76-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81a76-106">Permission type</span></span>      | <span data-ttu-id="81a76-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81a76-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81a76-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81a76-108">Delegated (work or school account)</span></span> | <span data-ttu-id="81a76-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81a76-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81a76-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81a76-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81a76-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81a76-111">Not supported.</span></span>    |
|<span data-ttu-id="81a76-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81a76-112">Application</span></span> | <span data-ttu-id="81a76-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81a76-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81a76-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81a76-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="81a76-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81a76-115">Optional request headers</span></span>
| <span data-ttu-id="81a76-116">Name</span><span class="sxs-lookup"><span data-stu-id="81a76-116">Name</span></span>       | <span data-ttu-id="81a76-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a76-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="81a76-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a76-118">Authorization</span></span>  | <span data-ttu-id="81a76-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="81a76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81a76-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81a76-121">Request body</span></span>
<span data-ttu-id="81a76-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="81a76-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="81a76-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81a76-125">Property</span></span>     | <span data-ttu-id="81a76-126">Typ</span><span class="sxs-lookup"><span data-stu-id="81a76-126">Type</span></span>   |<span data-ttu-id="81a76-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a76-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a76-128">name</span><span class="sxs-lookup"><span data-stu-id="81a76-128">name</span></span>|<span data-ttu-id="81a76-129">string</span><span class="sxs-lookup"><span data-stu-id="81a76-129">string</span></span>|<span data-ttu-id="81a76-130">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="81a76-130">The display name of the worksheet.</span></span>|
|<span data-ttu-id="81a76-131">position</span><span class="sxs-lookup"><span data-stu-id="81a76-131">position</span></span>|<span data-ttu-id="81a76-132">int</span><span class="sxs-lookup"><span data-stu-id="81a76-132">int</span></span>|<span data-ttu-id="81a76-133">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="81a76-133">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="81a76-134">visibility</span><span class="sxs-lookup"><span data-stu-id="81a76-134">visibility</span></span>|<span data-ttu-id="81a76-135">string</span><span class="sxs-lookup"><span data-stu-id="81a76-135">string</span></span>|<span data-ttu-id="81a76-p104">Die Sichtbarkeit des Arbeitsblatts. Mögliche Werte: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="81a76-p104">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="81a76-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="81a76-138">Response</span></span>

<span data-ttu-id="81a76-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Worksheet](../resources/worksheet.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81a76-139">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81a76-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81a76-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81a76-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81a76-141">Request</span></span>
<span data-ttu-id="81a76-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81a76-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="81a76-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="81a76-143">Response</span></span>
<span data-ttu-id="81a76-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81a76-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
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