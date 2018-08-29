# <a name="table-headerrowrange"></a><span data-ttu-id="b9607-101">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="b9607-101">Table: HeaderRowRange</span></span>

<span data-ttu-id="b9607-102">Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="b9607-102">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9607-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9607-103">Permissions</span></span>
<span data-ttu-id="b9607-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9607-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9607-106">Permission type</span></span>      | <span data-ttu-id="b9607-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9607-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9607-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9607-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9607-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9607-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9607-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9607-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9607-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9607-111">Not supported.</span></span>    |
|<span data-ttu-id="b9607-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9607-112">Application</span></span> | <span data-ttu-id="b9607-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9607-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9607-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9607-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="b9607-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9607-115">Request headers</span></span>
| <span data-ttu-id="b9607-116">Name</span><span class="sxs-lookup"><span data-stu-id="b9607-116">Name</span></span>       | <span data-ttu-id="b9607-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9607-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9607-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b9607-118">Authorization</span></span>  | <span data-ttu-id="b9607-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9607-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9607-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b9607-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9607-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b9607-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9607-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9607-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b9607-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9607-125">Response</span></span>

<span data-ttu-id="b9607-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9607-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9607-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9607-127">Example</span></span>
<span data-ttu-id="b9607-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b9607-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9607-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9607-129">Request</span></span>
<span data-ttu-id="b9607-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9607-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```

##### <a name="response"></a><span data-ttu-id="b9607-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9607-131">Response</span></span>
<span data-ttu-id="b9607-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9607-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->