# <a name="workbookrange-resizedrange"></a><span data-ttu-id="63fc3-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="63fc3-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="63fc3-102">Ruft ein Range-Objekt ähnlich dem aktuellen Range-Objekt ab, dessen untere rechte Ecke jedoch um eine bestimmte Anzahl von Zeilen und Spalten erweitert (oder verkleinert) ist.</span><span class="sxs-lookup"><span data-stu-id="63fc3-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="63fc3-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="63fc3-103">Permissions</span></span>
<span data-ttu-id="63fc3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63fc3-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63fc3-106">Permission type</span></span>      | <span data-ttu-id="63fc3-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63fc3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63fc3-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63fc3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="63fc3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63fc3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63fc3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63fc3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63fc3-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63fc3-111">Not supported.</span></span>    |
|<span data-ttu-id="63fc3-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63fc3-112">Application</span></span> | <span data-ttu-id="63fc3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63fc3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63fc3-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63fc3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="63fc3-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63fc3-115">Request headers</span></span>
| <span data-ttu-id="63fc3-116">Name</span><span class="sxs-lookup"><span data-stu-id="63fc3-116">Name</span></span>       | <span data-ttu-id="63fc3-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63fc3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63fc3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="63fc3-118">Authorization</span></span>  | <span data-ttu-id="63fc3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63fc3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63fc3-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="63fc3-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="63fc3-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="63fc3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="63fc3-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="63fc3-124">Parameters</span></span>

| <span data-ttu-id="63fc3-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="63fc3-125">Parameter</span></span>    | <span data-ttu-id="63fc3-126">Typ</span><span class="sxs-lookup"><span data-stu-id="63fc3-126">Type</span></span>   |<span data-ttu-id="63fc3-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63fc3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63fc3-128">deltarows</span><span class="sxs-lookup"><span data-stu-id="63fc3-128">deltarows</span></span>|<span data-ttu-id="63fc3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="63fc3-129">Int32</span></span>|<span data-ttu-id="63fc3-p104">Die Anzahl von Zeilen, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="63fc3-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="63fc3-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="63fc3-132">deltaColumns</span></span>|<span data-ttu-id="63fc3-133">Int32</span><span class="sxs-lookup"><span data-stu-id="63fc3-133">Int32</span></span>|<span data-ttu-id="63fc3-p105">Die Anzahl von Spalten, um die die untere rechte Ecke relativ zum aktuellen Bereich zu erweitern ist. Verwenden Sie eine positive Zahl, um den Bereich zu erweitern, oder eine negative Zahl, um ihn zu verkleinern.</span><span class="sxs-lookup"><span data-stu-id="63fc3-p105">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63fc3-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63fc3-136">Request body</span></span>
<span data-ttu-id="63fc3-137">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="63fc3-137">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="63fc3-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="63fc3-138">Parameter</span></span>    | <span data-ttu-id="63fc3-139">Typ</span><span class="sxs-lookup"><span data-stu-id="63fc3-139">Type</span></span>   |<span data-ttu-id="63fc3-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63fc3-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63fc3-141">deltaRows</span><span class="sxs-lookup"><span data-stu-id="63fc3-141">deltaRows</span></span>|<span data-ttu-id="63fc3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="63fc3-142">Int32</span></span>||
|<span data-ttu-id="63fc3-143">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="63fc3-143">deltaColumns</span></span>|<span data-ttu-id="63fc3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="63fc3-144">Int32</span></span>||

### <a name="response"></a><span data-ttu-id="63fc3-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="63fc3-145">Response</span></span>
<span data-ttu-id="63fc3-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63fc3-146">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63fc3-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63fc3-147">Example</span></span>
<span data-ttu-id="63fc3-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="63fc3-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63fc3-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63fc3-149">Request</span></span>
<span data-ttu-id="63fc3-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63fc3-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="63fc3-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="63fc3-151">Response</span></span>
<span data-ttu-id="63fc3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63fc3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
