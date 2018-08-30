# <a name="workbookrange-resizedrange"></a><span data-ttu-id="cbbdb-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="cbbdb-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="cbbdb-102">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbbdb-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cbbdb-103">Permissions</span></span>
<span data-ttu-id="cbbdb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbbdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cbbdb-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbbdb-106">Permission type</span></span>      | <span data-ttu-id="cbbdb-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbbdb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbbdb-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbbdb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cbbdb-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbbdb-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbbdb-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbbdb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbbdb-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbbdb-111">Not supported.</span></span>    |
|<span data-ttu-id="cbbdb-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-112">Application</span></span> | <span data-ttu-id="cbbdb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbbdb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbbdb-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="cbbdb-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbbdb-115">Request headers</span></span>
| <span data-ttu-id="cbbdb-116">Name</span><span class="sxs-lookup"><span data-stu-id="cbbdb-116">Name</span></span>       | <span data-ttu-id="cbbdb-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbbdb-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-118">Authorization</span></span>  | <span data-ttu-id="cbbdb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbbdb-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cbbdb-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbbdb-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="cbbdb-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="cbbdb-124">Parameters</span></span>

| <span data-ttu-id="cbbdb-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="cbbdb-125">Parameter</span></span>    | <span data-ttu-id="cbbdb-126">Typ</span><span class="sxs-lookup"><span data-stu-id="cbbdb-126">Type</span></span>   |<span data-ttu-id="cbbdb-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbbdb-128">deltaRows</span><span class="sxs-lookup"><span data-stu-id="cbbdb-128">deltaRows</span></span>|<span data-ttu-id="cbbdb-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cbbdb-129">Int32</span></span>|<span data-ttu-id="cbbdb-p104">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="cbbdb-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="cbbdb-132">deltaColumns</span></span>|<span data-ttu-id="cbbdb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cbbdb-133">Int32</span></span>|<span data-ttu-id="cbbdb-134">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-134">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span> <span data-ttu-id="cbbdb-135">Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-135">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

### <a name="response"></a><span data-ttu-id="cbbdb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbbdb-136">Response</span></span>
<span data-ttu-id="cbbdb-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbbdb-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbbdb-138">Example</span></span>
<span data-ttu-id="cbbdb-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cbbdb-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbbdb-140">Request</span></span>
<span data-ttu-id="cbbdb-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="cbbdb-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbbdb-142">Response</span></span>
<span data-ttu-id="cbbdb-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbbdb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
