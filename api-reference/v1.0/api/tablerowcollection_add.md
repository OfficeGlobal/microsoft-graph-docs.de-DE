# <a name="tablerowcollection-add"></a><span data-ttu-id="c08de-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="c08de-101">TableRowCollection: add</span></span>

<span data-ttu-id="c08de-102">Fügt der Tabelle eine neue Zeile hinzu.</span><span class="sxs-lookup"><span data-stu-id="c08de-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c08de-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c08de-103">Permissions</span></span>
<span data-ttu-id="c08de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c08de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c08de-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c08de-106">Permission type</span></span>      | <span data-ttu-id="c08de-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c08de-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c08de-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c08de-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c08de-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c08de-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c08de-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c08de-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c08de-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c08de-111">Not supported.</span></span>    |
|<span data-ttu-id="c08de-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c08de-112">Application</span></span> | <span data-ttu-id="c08de-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c08de-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c08de-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c08de-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="c08de-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c08de-115">Request headers</span></span>
| <span data-ttu-id="c08de-116">Name</span><span class="sxs-lookup"><span data-stu-id="c08de-116">Name</span></span>       | <span data-ttu-id="c08de-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c08de-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c08de-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c08de-118">Authorization</span></span>  | <span data-ttu-id="c08de-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c08de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c08de-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c08de-121">Request body</span></span>
<span data-ttu-id="c08de-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c08de-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c08de-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="c08de-123">Parameter</span></span>    | <span data-ttu-id="c08de-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c08de-124">Type</span></span>   |<span data-ttu-id="c08de-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c08de-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c08de-126">Index</span><span class="sxs-lookup"><span data-stu-id="c08de-126">index</span></span>|<span data-ttu-id="c08de-127">number</span><span class="sxs-lookup"><span data-stu-id="c08de-127">number</span></span>|<span data-ttu-id="c08de-p103">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="c08de-p103">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="c08de-133">values</span><span class="sxs-lookup"><span data-stu-id="c08de-133">values</span></span>|<span data-ttu-id="c08de-134">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="c08de-134">(boolean or string or number)</span></span>|<span data-ttu-id="c08de-p104">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenzeile.</span><span class="sxs-lookup"><span data-stu-id="c08de-p104">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="c08de-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c08de-137">Response</span></span>

<span data-ttu-id="c08de-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c08de-138">If successful, this method returns `200, OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c08de-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c08de-139">Example</span></span>
<span data-ttu-id="c08de-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c08de-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c08de-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c08de-141">Request</span></span>
<span data-ttu-id="c08de-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c08de-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="c08de-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c08de-143">Response</span></span>
<span data-ttu-id="c08de-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c08de-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
