# <a name="worksheet-cell"></a><span data-ttu-id="57a3d-101">Arbeitsblatt: Zelle</span><span class="sxs-lookup"><span data-stu-id="57a3d-101">Worksheet: Cell</span></span>

<span data-ttu-id="57a3d-p101">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="57a3d-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57a3d-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57a3d-104">Prerequisites</span></span>
<span data-ttu-id="57a3d-105">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="57a3d-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="57a3d-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57a3d-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="57a3d-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57a3d-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="57a3d-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57a3d-108">Request headers</span></span>
| <span data-ttu-id="57a3d-109">Name</span><span class="sxs-lookup"><span data-stu-id="57a3d-109">Name</span></span>       | <span data-ttu-id="57a3d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57a3d-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57a3d-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="57a3d-111">Authorization</span></span>  | <span data-ttu-id="57a3d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="57a3d-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="57a3d-114">Antwort</span><span class="sxs-lookup"><span data-stu-id="57a3d-114">Response</span></span>

<span data-ttu-id="57a3d-115">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57a3d-115">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57a3d-116">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57a3d-116">Example</span></span>
<span data-ttu-id="57a3d-117">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="57a3d-117">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57a3d-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57a3d-118">Request</span></span>
<span data-ttu-id="57a3d-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57a3d-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="57a3d-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="57a3d-120">Response</span></span>
<span data-ttu-id="57a3d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57a3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
