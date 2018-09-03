# <a name="workbookrange-rowsabove"></a><span data-ttu-id="fcc60-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="fcc60-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="fcc60-102">Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="fcc60-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcc60-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fcc60-103">Permissions</span></span>
<span data-ttu-id="fcc60-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcc60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcc60-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fcc60-106">Permission type</span></span>      | <span data-ttu-id="fcc60-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fcc60-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcc60-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fcc60-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fcc60-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcc60-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fcc60-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fcc60-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcc60-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcc60-111">Not supported.</span></span>    |
|<span data-ttu-id="fcc60-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fcc60-112">Application</span></span> | <span data-ttu-id="fcc60-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcc60-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcc60-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcc60-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="fcc60-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fcc60-115">Request headers</span></span>
| <span data-ttu-id="fcc60-116">Name</span><span class="sxs-lookup"><span data-stu-id="fcc60-116">Name</span></span>       | <span data-ttu-id="fcc60-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcc60-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fcc60-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fcc60-118">Authorization</span></span>  | <span data-ttu-id="fcc60-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fcc60-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcc60-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fcc60-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fcc60-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fcc60-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="fcc60-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="fcc60-124">Parameters</span></span>

| <span data-ttu-id="fcc60-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="fcc60-125">Parameter</span></span>    | <span data-ttu-id="fcc60-126">Typ</span><span class="sxs-lookup"><span data-stu-id="fcc60-126">Type</span></span>   |<span data-ttu-id="fcc60-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcc60-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcc60-128">Anzahl</span><span class="sxs-lookup"><span data-stu-id="fcc60-128">count</span></span>|<span data-ttu-id="fcc60-129">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc60-129">Int32</span></span>|<span data-ttu-id="fcc60-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="fcc60-130">Optional.</span></span> <span data-ttu-id="fcc60-131">Die Anzahl der Zeilen, die im resultierenden Bereich aufgenommen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="fcc60-131">The number of rows to include in the resulting range.</span></span> <span data-ttu-id="fcc60-132">Verwenden Sie im Allgemeinen eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="fcc60-132">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="fcc60-133">Sie können auch eine negative Zahl verwenden, um einen Bereich im aktuellen Bereich zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="fcc60-133">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="fcc60-134">Der Standardwert ist 1</span><span class="sxs-lookup"><span data-stu-id="fcc60-134">The default value is 1.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcc60-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fcc60-135">Request body</span></span>

### <a name="response"></a><span data-ttu-id="fcc60-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcc60-136">Response</span></span>
<span data-ttu-id="fcc60-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcc60-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcc60-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fcc60-138">Example</span></span>
<span data-ttu-id="fcc60-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fcc60-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fcc60-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcc60-140">Request</span></span>
<span data-ttu-id="fcc60-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fcc60-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="fcc60-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcc60-142">Response</span></span>
<span data-ttu-id="fcc60-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcc60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="fcc60-146">Wenn ohne den optionalen `count` Parameter aufgerufen, gibt diese Funktion nur eine Zeile oberhalb des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="fcc60-146">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="fcc60-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcc60-147">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="fcc60-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcc60-148">Response</span></span>
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