# <a name="chart-setposition"></a><span data-ttu-id="4d049-101">Diagramm: SetPosition</span><span class="sxs-lookup"><span data-stu-id="4d049-101">Chart: setPosition</span></span>

<span data-ttu-id="4d049-102">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="4d049-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d049-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d049-103">Permissions</span></span>
<span data-ttu-id="4d049-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d049-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d049-106">Permission type</span></span>      | <span data-ttu-id="4d049-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d049-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d049-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d049-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4d049-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d049-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d049-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d049-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d049-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d049-111">Not supported.</span></span>    |
|<span data-ttu-id="4d049-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d049-112">Application</span></span> | <span data-ttu-id="4d049-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d049-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d049-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d049-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="4d049-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d049-115">Request headers</span></span>
| <span data-ttu-id="4d049-116">Name</span><span class="sxs-lookup"><span data-stu-id="4d049-116">Name</span></span>       | <span data-ttu-id="4d049-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d049-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d049-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4d049-118">Authorization</span></span>  | <span data-ttu-id="4d049-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d049-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d049-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4d049-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d049-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4d049-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d049-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d049-124">Request body</span></span>
<span data-ttu-id="4d049-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4d049-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d049-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="4d049-126">Parameter</span></span>    | <span data-ttu-id="4d049-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4d049-127">Type</span></span>   |<span data-ttu-id="4d049-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d049-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d049-129">startCell</span><span class="sxs-lookup"><span data-stu-id="4d049-129">startCell</span></span>|<span data-ttu-id="4d049-130">Json</span><span class="sxs-lookup"><span data-stu-id="4d049-130">Json</span></span>|<span data-ttu-id="4d049-p104">Die Startzelle. An diese Position wird das Diagramm verschoben. Die Startzelle ist die obere linke oder die obere rechte Zelle, abhängig davon, ob die eingestellte Textrichtung des Benutzers von links nach rechts oder von rechts nach links ist.</span><span class="sxs-lookup"><span data-stu-id="4d049-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="4d049-134">endCell</span><span class="sxs-lookup"><span data-stu-id="4d049-134">endCell</span></span>|<span data-ttu-id="4d049-135">Json</span><span class="sxs-lookup"><span data-stu-id="4d049-135">Json</span></span>|<span data-ttu-id="4d049-p105">Optional. Die Endzelle. Wenn angegeben, werden Breite und Höhe des Diagramms so eingestellt, dass diese Zelle/dieser Bereich vollständig bedeckt ist.</span><span class="sxs-lookup"><span data-stu-id="4d049-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="4d049-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d049-139">Response</span></span>

<span data-ttu-id="4d049-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d049-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d049-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d049-142">Example</span></span>
<span data-ttu-id="4d049-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4d049-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d049-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d049-144">Request</span></span>
<span data-ttu-id="4d049-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d049-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="4d049-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d049-146">Response</span></span>
<span data-ttu-id="4d049-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4d049-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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