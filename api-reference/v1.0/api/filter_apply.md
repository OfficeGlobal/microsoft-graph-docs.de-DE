# <a name="filter-apply"></a><span data-ttu-id="a8aa4-101">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="a8aa4-101">Filter: apply</span></span>

<span data-ttu-id="a8aa4-102">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-102">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8aa4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8aa4-103">Permissions</span></span>
<span data-ttu-id="a8aa4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8aa4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8aa4-106">Permission type</span></span>      | <span data-ttu-id="a8aa4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8aa4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8aa4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8aa4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a8aa4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8aa4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8aa4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8aa4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8aa4-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8aa4-111">Not supported.</span></span>    |
|<span data-ttu-id="a8aa4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8aa4-112">Application</span></span> | <span data-ttu-id="a8aa4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8aa4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8aa4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8aa4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="a8aa4-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8aa4-115">Request headers</span></span>
| <span data-ttu-id="a8aa4-116">Name</span><span class="sxs-lookup"><span data-stu-id="a8aa4-116">Name</span></span>       | <span data-ttu-id="a8aa4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8aa4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8aa4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8aa4-118">Authorization</span></span>  | <span data-ttu-id="a8aa4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8aa4-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8aa4-121">Request body</span></span>
<span data-ttu-id="a8aa4-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8aa4-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8aa4-123">Parameter</span></span>    | <span data-ttu-id="a8aa4-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a8aa4-124">Type</span></span>   |<span data-ttu-id="a8aa4-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8aa4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8aa4-126">criteria</span><span class="sxs-lookup"><span data-stu-id="a8aa4-126">criteria</span></span>|<span data-ttu-id="a8aa4-127">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="a8aa4-127">FilterCriteria</span></span>|<span data-ttu-id="a8aa4-128">Die Kriterien, die angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-128">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="a8aa4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8aa4-129">Response</span></span>

<span data-ttu-id="a8aa4-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8aa4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8aa4-132">Example</span></span>
<span data-ttu-id="a8aa4-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8aa4-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8aa4-134">Request</span></span>
<span data-ttu-id="a8aa4-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a8aa4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8aa4-136">Response</span></span>
<span data-ttu-id="a8aa4-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8aa4-137">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->