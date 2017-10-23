# <a name="add-named-item"></a><span data-ttu-id="6412c-101">Benanntes Element hinzufügen</span><span class="sxs-lookup"><span data-stu-id="6412c-101">Add Named Item</span></span>

<span data-ttu-id="6412c-102">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="6412c-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="6412c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6412c-103">Permissions</span></span>
<span data-ttu-id="6412c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6412c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6412c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6412c-106">Permission type</span></span>      | <span data-ttu-id="6412c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6412c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6412c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6412c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6412c-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6412c-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="6412c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6412c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6412c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6412c-111">Not supported.</span></span>    |
|<span data-ttu-id="6412c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6412c-112">Application</span></span> | <span data-ttu-id="6412c-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6412c-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6412c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6412c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="6412c-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6412c-115">Request headers</span></span>
| <span data-ttu-id="6412c-116">Name</span><span class="sxs-lookup"><span data-stu-id="6412c-116">Name</span></span>       | <span data-ttu-id="6412c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6412c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6412c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6412c-118">Authorization</span></span>  | <span data-ttu-id="6412c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6412c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6412c-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6412c-121">Request body</span></span>
<span data-ttu-id="6412c-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6412c-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6412c-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="6412c-123">Parameter</span></span>    | <span data-ttu-id="6412c-124">Typ</span><span class="sxs-lookup"><span data-stu-id="6412c-124">Type</span></span>   |<span data-ttu-id="6412c-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6412c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6412c-126">name</span><span class="sxs-lookup"><span data-stu-id="6412c-126">name</span></span>|<span data-ttu-id="6412c-127">string</span><span class="sxs-lookup"><span data-stu-id="6412c-127">string</span></span>|<span data-ttu-id="6412c-128">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="6412c-128">The name of the named item.</span></span>|
|<span data-ttu-id="6412c-129">Referenz</span><span class="sxs-lookup"><span data-stu-id="6412c-129">reference</span></span>|<span data-ttu-id="6412c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6412c-130">string</span></span>|<span data-ttu-id="6412c-131">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="6412c-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="6412c-132">Kommentar</span><span class="sxs-lookup"><span data-stu-id="6412c-132">comment</span></span>|<span data-ttu-id="6412c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6412c-133">string</span></span>|<span data-ttu-id="6412c-134">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="6412c-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="6412c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6412c-135">Response</span></span>

<span data-ttu-id="6412c-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/NamedItem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6412c-136">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="6412c-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6412c-137">Example</span></span>
<span data-ttu-id="6412c-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6412c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6412c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6412c-139">Request</span></span>
<span data-ttu-id="6412c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6412c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="6412c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="6412c-141">Response</span></span>
<span data-ttu-id="6412c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6412c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
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
