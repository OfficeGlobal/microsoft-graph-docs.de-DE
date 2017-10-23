# <a name="range-delete"></a><span data-ttu-id="4bee2-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="4bee2-101">Range: delete</span></span>

<span data-ttu-id="4bee2-102">Löscht die einem Bereich zugeordneten Zellen.</span><span class="sxs-lookup"><span data-stu-id="4bee2-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bee2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4bee2-103">Permissions</span></span>
<span data-ttu-id="4bee2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bee2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bee2-106">Permission type</span></span>      | <span data-ttu-id="4bee2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bee2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bee2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bee2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4bee2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bee2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4bee2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bee2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bee2-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bee2-111">Not supported.</span></span>    |
|<span data-ttu-id="4bee2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bee2-112">Application</span></span> | <span data-ttu-id="4bee2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bee2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bee2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bee2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="4bee2-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bee2-115">Request headers</span></span>
| <span data-ttu-id="4bee2-116">Name</span><span class="sxs-lookup"><span data-stu-id="4bee2-116">Name</span></span>       | <span data-ttu-id="4bee2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bee2-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bee2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bee2-118">Authorization</span></span>  | <span data-ttu-id="4bee2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4bee2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bee2-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bee2-121">Request body</span></span>
<span data-ttu-id="4bee2-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4bee2-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bee2-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="4bee2-123">Parameter</span></span>    | <span data-ttu-id="4bee2-124">Typ</span><span class="sxs-lookup"><span data-stu-id="4bee2-124">Type</span></span>   |<span data-ttu-id="4bee2-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bee2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bee2-126">Shift</span><span class="sxs-lookup"><span data-stu-id="4bee2-126">shift</span></span>|<span data-ttu-id="4bee2-127">string</span><span class="sxs-lookup"><span data-stu-id="4bee2-127">string</span></span>|<span data-ttu-id="4bee2-p103">Gibt an, wohin die Zellen verschoben werden.  Mögliche Werte: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="4bee2-p103">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="4bee2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bee2-130">Response</span></span>

<span data-ttu-id="4bee2-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bee2-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bee2-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bee2-133">Example</span></span>
<span data-ttu-id="4bee2-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4bee2-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bee2-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bee2-135">Request</span></span>
<span data-ttu-id="4bee2-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4bee2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="4bee2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bee2-137">Response</span></span>
<span data-ttu-id="4bee2-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4bee2-138">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->