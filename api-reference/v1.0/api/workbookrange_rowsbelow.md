# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="06575-101">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="06575-101">workbookRange: rowsBelow</span></span>

<span data-ttu-id="06575-102">Ruft eine bestimmte Anzahl von Zeilen unterhalb eines gegebenen Bereichs ab.</span><span class="sxs-lookup"><span data-stu-id="06575-102">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="06575-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06575-103">Permissions</span></span>
<span data-ttu-id="06575-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06575-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06575-106">Permission type</span></span>      | <span data-ttu-id="06575-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06575-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06575-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06575-108">Delegated (work or school account)</span></span> | <span data-ttu-id="06575-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06575-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06575-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06575-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06575-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06575-111">Not supported.</span></span>    |
|<span data-ttu-id="06575-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06575-112">Application</span></span> | <span data-ttu-id="06575-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06575-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06575-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06575-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="06575-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06575-115">Request headers</span></span>
| <span data-ttu-id="06575-116">Name</span><span class="sxs-lookup"><span data-stu-id="06575-116">Name</span></span>       | <span data-ttu-id="06575-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06575-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06575-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="06575-118">Authorization</span></span>  | <span data-ttu-id="06575-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06575-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06575-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="06575-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="06575-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="06575-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="06575-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="06575-124">Parameters</span></span>

| <span data-ttu-id="06575-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="06575-125">Parameter</span></span>    | <span data-ttu-id="06575-126">Typ</span><span class="sxs-lookup"><span data-stu-id="06575-126">Type</span></span>   |<span data-ttu-id="06575-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06575-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06575-128">count</span><span class="sxs-lookup"><span data-stu-id="06575-128">count</span></span>|<span data-ttu-id="06575-129">Int32</span><span class="sxs-lookup"><span data-stu-id="06575-129">Int32</span></span>|<span data-ttu-id="06575-p104">Die Anzahl von Zeilen, die in den Ergebnisbereich aufgenommen werden soll. Grundsätzlich verwenden Sie eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs zu erstellen. Sie können auch eine negative Zahl verwenden, um einen Bereich innerhalb des aktuellen Bereichs zu erstellen. Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="06575-p104">The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="06575-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06575-134">Request body</span></span>

### <a name="response"></a><span data-ttu-id="06575-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="06575-135">Response</span></span>
<span data-ttu-id="06575-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06575-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06575-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06575-137">Example</span></span>
<span data-ttu-id="06575-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="06575-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06575-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06575-139">Request</span></span>
<span data-ttu-id="06575-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06575-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="06575-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="06575-141">Response</span></span>
<span data-ttu-id="06575-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06575-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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