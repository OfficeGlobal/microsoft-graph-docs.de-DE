# <a name="table-headerrowrange"></a><span data-ttu-id="2a5a3-101">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="2a5a3-101">Table: HeaderRowRange</span></span>

<span data-ttu-id="2a5a3-102">Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-102">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a5a3-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a5a3-103">Permissions</span></span>
<span data-ttu-id="2a5a3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a5a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a5a3-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a5a3-106">Permission type</span></span>      | <span data-ttu-id="2a5a3-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a5a3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a5a3-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a5a3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2a5a3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a5a3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a5a3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a5a3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a5a3-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a5a3-111">Not supported.</span></span>    |
|<span data-ttu-id="2a5a3-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a5a3-112">Application</span></span> | <span data-ttu-id="2a5a3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a5a3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a5a3-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a5a3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="2a5a3-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a5a3-115">Request headers</span></span>
| <span data-ttu-id="2a5a3-116">Name</span><span class="sxs-lookup"><span data-stu-id="2a5a3-116">Name</span></span>       | <span data-ttu-id="2a5a3-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a5a3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a5a3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a5a3-118">Authorization</span></span>  | <span data-ttu-id="2a5a3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a5a3-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a5a3-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2a5a3-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a5a3-122">Response</span></span>

<span data-ttu-id="2a5a3-123">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-123">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a5a3-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a5a3-124">Example</span></span>
<span data-ttu-id="2a5a3-125">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2a5a3-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a5a3-126">Request</span></span>
<span data-ttu-id="2a5a3-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="2a5a3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a5a3-128">Response</span></span>
<span data-ttu-id="2a5a3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a5a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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