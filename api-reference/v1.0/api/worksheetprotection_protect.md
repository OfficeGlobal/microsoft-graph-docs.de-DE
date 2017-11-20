# <a name="worksheetprotection-protect"></a><span data-ttu-id="5d4b8-101">WorksheetProtection: Schützen</span><span class="sxs-lookup"><span data-stu-id="5d4b8-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="5d4b8-p101">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d4b8-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d4b8-104">Permissions</span></span>
<span data-ttu-id="5d4b8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d4b8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d4b8-107">Permission type</span></span>      | <span data-ttu-id="5d4b8-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d4b8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d4b8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d4b8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5d4b8-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d4b8-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d4b8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d4b8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d4b8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d4b8-112">Not supported.</span></span>    |
|<span data-ttu-id="5d4b8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d4b8-113">Application</span></span> | <span data-ttu-id="5d4b8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d4b8-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d4b8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d4b8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="5d4b8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d4b8-116">Request headers</span></span>
| <span data-ttu-id="5d4b8-117">Name</span><span class="sxs-lookup"><span data-stu-id="5d4b8-117">Name</span></span>       | <span data-ttu-id="5d4b8-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d4b8-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d4b8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d4b8-119">Authorization</span></span>  | <span data-ttu-id="5d4b8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d4b8-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5d4b8-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="5d4b8-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d4b8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d4b8-125">Request body</span></span>
<span data-ttu-id="5d4b8-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d4b8-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="5d4b8-127">Parameter</span></span>    | <span data-ttu-id="5d4b8-128">Typ</span><span class="sxs-lookup"><span data-stu-id="5d4b8-128">Type</span></span>   |<span data-ttu-id="5d4b8-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d4b8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d4b8-130">options</span><span class="sxs-lookup"><span data-stu-id="5d4b8-130">options</span></span>|<span data-ttu-id="5d4b8-131">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="5d4b8-131">WorksheetProtectionOptions</span></span>|<span data-ttu-id="5d4b8-p105">Optional. Optionen für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p105">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="5d4b8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d4b8-134">Response</span></span>

<span data-ttu-id="5d4b8-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d4b8-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d4b8-137">Example</span></span>
<span data-ttu-id="5d4b8-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d4b8-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d4b8-139">Request</span></span>
<span data-ttu-id="5d4b8-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="5d4b8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d4b8-141">Response</span></span>
<span data-ttu-id="5d4b8-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d4b8-142">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
