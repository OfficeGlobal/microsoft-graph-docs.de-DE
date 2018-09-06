# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="4f7b5-101">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="4f7b5-101">workbookRange: rowsBelow</span></span>

<span data-ttu-id="4f7b5-102">Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-102">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f7b5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4f7b5-103">Permissions</span></span>
<span data-ttu-id="4f7b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f7b5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f7b5-106">Permission type</span></span>      | <span data-ttu-id="4f7b5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f7b5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f7b5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f7b5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4f7b5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f7b5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f7b5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f7b5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f7b5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f7b5-111">Not supported.</span></span>    |
|<span data-ttu-id="4f7b5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-112">Application</span></span> | <span data-ttu-id="4f7b5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f7b5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f7b5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="4f7b5-115">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4f7b5-115">Function parameters</span></span>

| <span data-ttu-id="4f7b5-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="4f7b5-116">Parameter</span></span>    | <span data-ttu-id="4f7b5-117">Typ</span><span class="sxs-lookup"><span data-stu-id="4f7b5-117">Type</span></span>   |<span data-ttu-id="4f7b5-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f7b5-119">count</span><span class="sxs-lookup"><span data-stu-id="4f7b5-119">count</span></span>|<span data-ttu-id="4f7b5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="4f7b5-120">Int32</span></span>| <span data-ttu-id="4f7b5-p102">Optional. Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4f7b5-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f7b5-126">Request headers</span></span>
| <span data-ttu-id="4f7b5-127">Name</span><span class="sxs-lookup"><span data-stu-id="4f7b5-127">Name</span></span>       | <span data-ttu-id="4f7b5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f7b5-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-129">Authorization</span></span>  | <span data-ttu-id="4f7b5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f7b5-132">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4f7b5-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f7b5-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f7b5-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f7b5-135">Request body</span></span>
<span data-ttu-id="4f7b5-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f7b5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f7b5-137">Response</span></span>
<span data-ttu-id="4f7b5-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f7b5-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f7b5-139">Example</span></span>
<span data-ttu-id="4f7b5-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f7b5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-141">Request</span></span>
<span data-ttu-id="4f7b5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="4f7b5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f7b5-143">Response</span></span>
<span data-ttu-id="4f7b5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="4f7b5-147">Wenn sie ohne die `count` -Parameter dieser Funktion aufgerufen wird, ist der Standard eine Zeile.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-147">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="4f7b5-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f7b5-148">Request</span></span>
<span data-ttu-id="4f7b5-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="4f7b5-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f7b5-150">Response</span></span>
<span data-ttu-id="4f7b5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f7b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
