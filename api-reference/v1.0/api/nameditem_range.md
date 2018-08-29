# <a name="nameditem-range"></a><span data-ttu-id="87c71-101">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="87c71-101">NamedItem: Range</span></span>

<span data-ttu-id="87c71-p101">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="87c71-p101">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="87c71-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87c71-104">Permissions</span></span>
<span data-ttu-id="87c71-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87c71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87c71-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87c71-107">Permission type</span></span>      | <span data-ttu-id="87c71-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87c71-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c71-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87c71-109">Delegated (work or school account)</span></span> | <span data-ttu-id="87c71-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87c71-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87c71-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87c71-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c71-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c71-112">Not supported.</span></span>    |
|<span data-ttu-id="87c71-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87c71-113">Application</span></span> | <span data-ttu-id="87c71-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c71-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c71-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c71-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="87c71-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87c71-116">Request headers</span></span>
| <span data-ttu-id="87c71-117">Name</span><span class="sxs-lookup"><span data-stu-id="87c71-117">Name</span></span>       | <span data-ttu-id="87c71-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c71-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87c71-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87c71-119">Authorization</span></span>  | <span data-ttu-id="87c71-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87c71-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87c71-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="87c71-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="87c71-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="87c71-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c71-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87c71-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="87c71-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c71-126">Response</span></span>

<span data-ttu-id="87c71-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c71-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87c71-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c71-128">Example</span></span>
<span data-ttu-id="87c71-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="87c71-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87c71-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c71-130">Request</span></span>
<span data-ttu-id="87c71-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c71-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="87c71-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c71-132">Response</span></span>
<span data-ttu-id="87c71-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c71-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->