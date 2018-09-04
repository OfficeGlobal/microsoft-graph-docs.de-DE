# <a name="workbookrange-rowsabove"></a><span data-ttu-id="e597b-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="e597b-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="e597b-102">Ruft eine bestimmte Anzahl von Zeilen oberhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="e597b-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e597b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e597b-103">Permissions</span></span>
<span data-ttu-id="e597b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e597b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e597b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e597b-106">Permission type</span></span>      | <span data-ttu-id="e597b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e597b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e597b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e597b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e597b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e597b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e597b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e597b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e597b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e597b-111">Not supported.</span></span>    |
|<span data-ttu-id="e597b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e597b-112">Application</span></span> | <span data-ttu-id="e597b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e597b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e597b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e597b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e597b-115">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e597b-115">Function parameters</span></span>

| <span data-ttu-id="e597b-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="e597b-116">Parameter</span></span>    | <span data-ttu-id="e597b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="e597b-117">Type</span></span>   |<span data-ttu-id="e597b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e597b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e597b-119">Anzahl</span><span class="sxs-lookup"><span data-stu-id="e597b-119">count</span></span>|<span data-ttu-id="e597b-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e597b-120">Int32</span></span>|<span data-ttu-id="e597b-p102">Optional. Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="e597b-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e597b-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e597b-126">Request headers</span></span>
| <span data-ttu-id="e597b-127">Name</span><span class="sxs-lookup"><span data-stu-id="e597b-127">Name</span></span>       | <span data-ttu-id="e597b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e597b-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e597b-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e597b-129">Authorization</span></span>  | <span data-ttu-id="e597b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e597b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e597b-132">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e597b-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="e597b-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e597b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e597b-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e597b-135">Request body</span></span>
<span data-ttu-id="e597b-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e597b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e597b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e597b-137">Response</span></span>
<span data-ttu-id="e597b-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e597b-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e597b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e597b-139">Example</span></span>
<span data-ttu-id="e597b-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e597b-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e597b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e597b-141">Request</span></span>
<span data-ttu-id="e597b-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e597b-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="e597b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e597b-143">Response</span></span>
<span data-ttu-id="e597b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e597b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="e597b-147">Ohne den optionalen `count` Parameter aufgerufen, gibt diese Funktion nur eine Zeile oberhalb des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="e597b-147">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="e597b-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e597b-148">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="e597b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e597b-149">Response</span></span>
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