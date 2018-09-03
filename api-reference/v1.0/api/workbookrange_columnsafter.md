# <a name="workbookrange-columnsafter"></a><span data-ttu-id="f5fbd-101">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="f5fbd-101">workbookRange: columnsAfter</span></span>

<span data-ttu-id="f5fbd-102">Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-102">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5fbd-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5fbd-103">Permissions</span></span>
<span data-ttu-id="f5fbd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5fbd-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5fbd-106">Permission type</span></span>      | <span data-ttu-id="f5fbd-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5fbd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5fbd-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5fbd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f5fbd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5fbd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5fbd-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5fbd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fbd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5fbd-111">Not supported.</span></span>    |
|<span data-ttu-id="f5fbd-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-112">Application</span></span> | <span data-ttu-id="f5fbd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5fbd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5fbd-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="f5fbd-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5fbd-115">Request headers</span></span>
| <span data-ttu-id="f5fbd-116">Name</span><span class="sxs-lookup"><span data-stu-id="f5fbd-116">Name</span></span>       | <span data-ttu-id="f5fbd-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5fbd-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-118">Authorization</span></span>  | <span data-ttu-id="f5fbd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5fbd-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f5fbd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5fbd-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="f5fbd-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="f5fbd-124">Parameters</span></span>

| <span data-ttu-id="f5fbd-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="f5fbd-125">Parameter</span></span>    | <span data-ttu-id="f5fbd-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f5fbd-126">Type</span></span>   |<span data-ttu-id="f5fbd-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5fbd-128">Anzahl</span><span class="sxs-lookup"><span data-stu-id="f5fbd-128">count</span></span>|<span data-ttu-id="f5fbd-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f5fbd-129">Int32</span></span>|<span data-ttu-id="f5fbd-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-130">Optional.</span></span> <span data-ttu-id="f5fbd-131">Die Anzahl der Zeilen, die im resultierenden Bereich aufgenommen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-131">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="f5fbd-132">Verwenden Sie im Allgemeinen eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-132">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="f5fbd-133">Sie können auch eine negative Zahl verwenden, um einen Bereich im aktuellen Bereich zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-133">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="f5fbd-134">Der Standardwert ist 1</span><span class="sxs-lookup"><span data-stu-id="f5fbd-134">The default value is 1.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5fbd-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5fbd-135">Request body</span></span>

### <a name="response"></a><span data-ttu-id="f5fbd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5fbd-136">Response</span></span>
<span data-ttu-id="f5fbd-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5fbd-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5fbd-138">Example</span></span>
<span data-ttu-id="f5fbd-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5fbd-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5fbd-140">Request</span></span>
<span data-ttu-id="f5fbd-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="f5fbd-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5fbd-142">Response</span></span>
<span data-ttu-id="f5fbd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5fbd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
