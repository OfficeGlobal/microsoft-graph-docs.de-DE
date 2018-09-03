# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="e439d-101">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="e439d-101">workbookRange: columnsBefore</span></span>

<span data-ttu-id="e439d-102">Ruft eine bestimmte Anzahl von Spalten links vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="e439d-102">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e439d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e439d-103">Permissions</span></span>
<span data-ttu-id="e439d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e439d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e439d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e439d-106">Permission type</span></span>      | <span data-ttu-id="e439d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e439d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e439d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e439d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e439d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e439d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e439d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e439d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e439d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e439d-111">Not supported.</span></span>    |
|<span data-ttu-id="e439d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e439d-112">Application</span></span> | <span data-ttu-id="e439d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e439d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e439d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e439d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="e439d-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e439d-115">Request headers</span></span>
| <span data-ttu-id="e439d-116">Name</span><span class="sxs-lookup"><span data-stu-id="e439d-116">Name</span></span>       | <span data-ttu-id="e439d-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e439d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e439d-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e439d-118">Authorization</span></span>  | <span data-ttu-id="e439d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e439d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e439d-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e439d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e439d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e439d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="e439d-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="e439d-124">Parameters</span></span>

| <span data-ttu-id="e439d-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="e439d-125">Parameter</span></span>    | <span data-ttu-id="e439d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e439d-126">Type</span></span>   |<span data-ttu-id="e439d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e439d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e439d-128">Anzahl</span><span class="sxs-lookup"><span data-stu-id="e439d-128">count</span></span>|<span data-ttu-id="e439d-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e439d-129">Int32</span></span>|<span data-ttu-id="e439d-p104">Optional. Die Anzahl von Spalten, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="e439d-p104">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e439d-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e439d-135">Request body</span></span>

### <a name="response"></a><span data-ttu-id="e439d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e439d-136">Response</span></span>
<span data-ttu-id="e439d-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e439d-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e439d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e439d-138">Example</span></span>
<span data-ttu-id="e439d-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e439d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e439d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e439d-140">Request</span></span>
<span data-ttu-id="e439d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e439d-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="e439d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e439d-142">Response</span></span>
<span data-ttu-id="e439d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e439d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
