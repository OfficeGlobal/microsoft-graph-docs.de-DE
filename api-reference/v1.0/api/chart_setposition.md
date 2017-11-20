# <a name="chart-setposition"></a><span data-ttu-id="a7f09-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="a7f09-101">Chart: setPosition</span></span>

<span data-ttu-id="a7f09-102">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="a7f09-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7f09-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a7f09-103">Permissions</span></span>
<span data-ttu-id="a7f09-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7f09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7f09-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7f09-106">Permission type</span></span>      | <span data-ttu-id="a7f09-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7f09-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7f09-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7f09-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a7f09-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7f09-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7f09-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7f09-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7f09-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7f09-111">Not supported.</span></span>    |
|<span data-ttu-id="a7f09-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7f09-112">Application</span></span> | <span data-ttu-id="a7f09-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7f09-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7f09-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7f09-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="a7f09-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7f09-115">Request headers</span></span>
| <span data-ttu-id="a7f09-116">Name</span><span class="sxs-lookup"><span data-stu-id="a7f09-116">Name</span></span>       | <span data-ttu-id="a7f09-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7f09-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7f09-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7f09-118">Authorization</span></span>  | <span data-ttu-id="a7f09-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7f09-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7f09-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a7f09-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7f09-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a7f09-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7f09-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7f09-124">Request body</span></span>
<span data-ttu-id="a7f09-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a7f09-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a7f09-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="a7f09-126">Parameter</span></span>    | <span data-ttu-id="a7f09-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a7f09-127">Type</span></span>   |<span data-ttu-id="a7f09-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7f09-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7f09-129">startCell</span><span class="sxs-lookup"><span data-stu-id="a7f09-129">startCell</span></span>|<span data-ttu-id="a7f09-130">string</span><span class="sxs-lookup"><span data-stu-id="a7f09-130">string</span></span>|<span data-ttu-id="a7f09-p104">Die Startzelle. An diese Position wird das Diagramm verschoben. Die Startzelle ist die obere linke oder die obere rechte Zelle, abhängig davon, ob die eingestellte Textrichtung des Benutzers von links nach rechts oder von rechts nach links ist.</span><span class="sxs-lookup"><span data-stu-id="a7f09-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="a7f09-134">endCell</span><span class="sxs-lookup"><span data-stu-id="a7f09-134">endCell</span></span>|<span data-ttu-id="a7f09-135">string</span><span class="sxs-lookup"><span data-stu-id="a7f09-135">string</span></span>|<span data-ttu-id="a7f09-p105">Optional. Die Endzelle. Wenn angegeben, werden Breite und Höhe des Diagramms so eingestellt, dass diese Zelle/dieser Bereich vollständig bedeckt ist.</span><span class="sxs-lookup"><span data-stu-id="a7f09-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="a7f09-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7f09-139">Response</span></span>

<span data-ttu-id="a7f09-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7f09-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7f09-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7f09-142">Example</span></span>
<span data-ttu-id="a7f09-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a7f09-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a7f09-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7f09-144">Request</span></span>
<span data-ttu-id="a7f09-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7f09-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="a7f09-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7f09-146">Response</span></span>
<span data-ttu-id="a7f09-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a7f09-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->