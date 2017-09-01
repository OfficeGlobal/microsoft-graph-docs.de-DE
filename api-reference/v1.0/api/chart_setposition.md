# <a name="chart-setposition"></a><span data-ttu-id="77d4b-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="77d4b-101">Chart: setPosition</span></span>

<span data-ttu-id="77d4b-102">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="77d4b-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="77d4b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77d4b-103">Permissions</span></span>
<span data-ttu-id="77d4b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77d4b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77d4b-106">Permission type</span></span>      | <span data-ttu-id="77d4b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77d4b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77d4b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77d4b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="77d4b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77d4b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77d4b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77d4b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77d4b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77d4b-111">Not supported.</span></span>    |
|<span data-ttu-id="77d4b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77d4b-112">Application</span></span> | <span data-ttu-id="77d4b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77d4b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77d4b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77d4b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="77d4b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77d4b-115">Request headers</span></span>
| <span data-ttu-id="77d4b-116">Name</span><span class="sxs-lookup"><span data-stu-id="77d4b-116">Name</span></span>       | <span data-ttu-id="77d4b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77d4b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77d4b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d4b-118">Authorization</span></span>  | <span data-ttu-id="77d4b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77d4b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77d4b-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77d4b-121">Request body</span></span>
<span data-ttu-id="77d4b-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="77d4b-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77d4b-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="77d4b-123">Parameter</span></span>    | <span data-ttu-id="77d4b-124">Typ</span><span class="sxs-lookup"><span data-stu-id="77d4b-124">Type</span></span>   |<span data-ttu-id="77d4b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77d4b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77d4b-126">startCell</span><span class="sxs-lookup"><span data-stu-id="77d4b-126">startCell</span></span>|<span data-ttu-id="77d4b-127">string</span><span class="sxs-lookup"><span data-stu-id="77d4b-127">string</span></span>|<span data-ttu-id="77d4b-p103">Die Startzelle. An diese Position wird das Diagramm verschoben. Die Startzelle ist die obere linke oder die obere rechte Zelle, abhängig davon, ob die eingestellte Textrichtung des Benutzers von links nach rechts oder von rechts nach links ist.</span><span class="sxs-lookup"><span data-stu-id="77d4b-p103">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="77d4b-131">endCell</span><span class="sxs-lookup"><span data-stu-id="77d4b-131">endCell</span></span>|<span data-ttu-id="77d4b-132">string</span><span class="sxs-lookup"><span data-stu-id="77d4b-132">string</span></span>|<span data-ttu-id="77d4b-p104">Optional. Die Endzelle. Wenn angegeben, werden Breite und Höhe des Diagramms so eingestellt, dass diese Zelle/dieser Bereich vollständig bedeckt ist.</span><span class="sxs-lookup"><span data-stu-id="77d4b-p104">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="77d4b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="77d4b-136">Response</span></span>

<span data-ttu-id="77d4b-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77d4b-p105">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d4b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77d4b-139">Example</span></span>
<span data-ttu-id="77d4b-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="77d4b-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="77d4b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77d4b-141">Request</span></span>
<span data-ttu-id="77d4b-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77d4b-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="77d4b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="77d4b-143">Response</span></span>
<span data-ttu-id="77d4b-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77d4b-144">Here is an example of the response.</span></span> 
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