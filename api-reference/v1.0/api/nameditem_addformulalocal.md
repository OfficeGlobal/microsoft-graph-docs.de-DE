# <a name="add-named-item-formulalocal"></a><span data-ttu-id="42147-101">Benanntes Element „FormulaLocal“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="42147-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="42147-102">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="42147-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="42147-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42147-103">Permissions</span></span>
<span data-ttu-id="42147-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="42147-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="42147-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42147-106">Permission type</span></span>      | <span data-ttu-id="42147-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42147-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42147-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42147-108">Delegated (work or school account)</span></span> | <span data-ttu-id="42147-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="42147-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="42147-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42147-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42147-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42147-111">Not supported.</span></span>    |
|<span data-ttu-id="42147-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42147-112">Application</span></span> | <span data-ttu-id="42147-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="42147-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42147-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42147-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="42147-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42147-115">Request headers</span></span>
| <span data-ttu-id="42147-116">Name</span><span class="sxs-lookup"><span data-stu-id="42147-116">Name</span></span>       | <span data-ttu-id="42147-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42147-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42147-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="42147-118">Authorization</span></span>  | <span data-ttu-id="42147-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42147-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42147-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42147-121">Request body</span></span>
<span data-ttu-id="42147-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="42147-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42147-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="42147-123">Parameter</span></span>    | <span data-ttu-id="42147-124">Typ</span><span class="sxs-lookup"><span data-stu-id="42147-124">Type</span></span>   |<span data-ttu-id="42147-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42147-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42147-126">name</span><span class="sxs-lookup"><span data-stu-id="42147-126">name</span></span>|<span data-ttu-id="42147-127">string</span><span class="sxs-lookup"><span data-stu-id="42147-127">string</span></span>|<span data-ttu-id="42147-128">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="42147-128">The name of the named item.</span></span>|
|<span data-ttu-id="42147-129">Formel</span><span class="sxs-lookup"><span data-stu-id="42147-129">formula</span></span>|<span data-ttu-id="42147-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42147-130">string</span></span>|<span data-ttu-id="42147-131">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="42147-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="42147-132">Kommentar</span><span class="sxs-lookup"><span data-stu-id="42147-132">comment</span></span>|<span data-ttu-id="42147-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42147-133">string</span></span>|<span data-ttu-id="42147-134">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="42147-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="42147-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="42147-135">Response</span></span>

<span data-ttu-id="42147-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/NamedItem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42147-136">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42147-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42147-137">Example</span></span>
<span data-ttu-id="42147-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="42147-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="42147-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42147-139">Request</span></span>
<span data-ttu-id="42147-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42147-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="42147-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="42147-141">Response</span></span>
<span data-ttu-id="42147-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42147-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
