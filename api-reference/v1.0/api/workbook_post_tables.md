# <a name="create-table"></a><span data-ttu-id="3bc94-101">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="3bc94-101">Create Table</span></span>

<span data-ttu-id="3bc94-102">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="3bc94-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bc94-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3bc94-103">Permissions</span></span>
<span data-ttu-id="3bc94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bc94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3bc94-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3bc94-106">Permission type</span></span>      | <span data-ttu-id="3bc94-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3bc94-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bc94-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3bc94-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3bc94-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bc94-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3bc94-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3bc94-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc94-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bc94-111">Not supported.</span></span>    |
|<span data-ttu-id="3bc94-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3bc94-112">Application</span></span> | <span data-ttu-id="3bc94-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3bc94-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bc94-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bc94-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="3bc94-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3bc94-115">Request headers</span></span>
| <span data-ttu-id="3bc94-116">Name</span><span class="sxs-lookup"><span data-stu-id="3bc94-116">Name</span></span>       | <span data-ttu-id="3bc94-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bc94-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3bc94-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bc94-118">Authorization</span></span>  | <span data-ttu-id="3bc94-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3bc94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bc94-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3bc94-121">Request body</span></span>
<span data-ttu-id="3bc94-122">Geben Sie im Anforderungstext eine JSON-Darstellung des [Table](../resources/table.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3bc94-122">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3bc94-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bc94-123">Response</span></span>

<span data-ttu-id="3bc94-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3bc94-124">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bc94-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3bc94-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bc94-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3bc94-126">Request</span></span>
<span data-ttu-id="3bc94-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3bc94-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="3bc94-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [Table](../resources/table.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3bc94-128">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3bc94-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3bc94-129">Response</span></span>
<span data-ttu-id="3bc94-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3bc94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
