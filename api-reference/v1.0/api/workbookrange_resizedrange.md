# <a name="workbookrange-resizedrange"></a><span data-ttu-id="23879-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="23879-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="23879-102">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="23879-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="23879-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23879-103">Permissions</span></span>
<span data-ttu-id="23879-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23879-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23879-106">Permission type</span></span>      | <span data-ttu-id="23879-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23879-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23879-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23879-108">Delegated (work or school account)</span></span> | <span data-ttu-id="23879-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23879-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23879-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23879-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23879-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23879-111">Not supported.</span></span>    |
|<span data-ttu-id="23879-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23879-112">Application</span></span> | <span data-ttu-id="23879-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23879-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23879-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23879-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="23879-115">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="23879-115">Function parameters</span></span>

| <span data-ttu-id="23879-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="23879-116">Parameter</span></span>    | <span data-ttu-id="23879-117">Typ</span><span class="sxs-lookup"><span data-stu-id="23879-117">Type</span></span>   |<span data-ttu-id="23879-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23879-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23879-119">deltaRows</span><span class="sxs-lookup"><span data-stu-id="23879-119">deltaRows</span></span>|<span data-ttu-id="23879-120">Int32</span><span class="sxs-lookup"><span data-stu-id="23879-120">Int32</span></span>|<span data-ttu-id="23879-p102">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="23879-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="23879-123">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="23879-123">deltaColumns</span></span>|<span data-ttu-id="23879-124">Int32</span><span class="sxs-lookup"><span data-stu-id="23879-124">Int32</span></span>|<span data-ttu-id="23879-125">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist.</span><span class="sxs-lookup"><span data-stu-id="23879-125">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span> <span data-ttu-id="23879-126">Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="23879-126">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="23879-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23879-127">Request headers</span></span>
| <span data-ttu-id="23879-128">Name</span><span class="sxs-lookup"><span data-stu-id="23879-128">Name</span></span>       | <span data-ttu-id="23879-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23879-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23879-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="23879-130">Authorization</span></span>  | <span data-ttu-id="23879-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23879-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23879-133">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="23879-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="23879-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="23879-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23879-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23879-136">Request body</span></span>
<span data-ttu-id="23879-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23879-137">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="23879-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="23879-138">Response</span></span>
<span data-ttu-id="23879-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23879-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23879-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23879-140">Example</span></span>
<span data-ttu-id="23879-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="23879-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23879-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23879-142">Request</span></span>
<span data-ttu-id="23879-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23879-143">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="23879-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="23879-144">Response</span></span>
<span data-ttu-id="23879-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23879-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
