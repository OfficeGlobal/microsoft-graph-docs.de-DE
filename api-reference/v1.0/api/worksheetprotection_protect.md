# <a name="worksheetprotection-protect"></a><span data-ttu-id="d3dba-101">WorksheetProtection: Schützen</span><span class="sxs-lookup"><span data-stu-id="d3dba-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="d3dba-p101">Schützen eines Arbeitsblatts. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="d3dba-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3dba-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d3dba-104">Permissions</span></span>
<span data-ttu-id="d3dba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3dba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3dba-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3dba-107">Permission type</span></span>      | <span data-ttu-id="d3dba-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3dba-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3dba-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3dba-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d3dba-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3dba-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3dba-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3dba-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3dba-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3dba-112">Not supported.</span></span>    |
|<span data-ttu-id="d3dba-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3dba-113">Application</span></span> | <span data-ttu-id="d3dba-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3dba-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3dba-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3dba-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d3dba-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3dba-116">Request headers</span></span>
| <span data-ttu-id="d3dba-117">Name</span><span class="sxs-lookup"><span data-stu-id="d3dba-117">Name</span></span>       | <span data-ttu-id="d3dba-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3dba-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3dba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3dba-119">Authorization</span></span>  | <span data-ttu-id="d3dba-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3dba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3dba-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3dba-122">Request body</span></span>
<span data-ttu-id="d3dba-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d3dba-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3dba-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="d3dba-124">Parameter</span></span>    | <span data-ttu-id="d3dba-125">Typ</span><span class="sxs-lookup"><span data-stu-id="d3dba-125">Type</span></span>   |<span data-ttu-id="d3dba-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3dba-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3dba-127">options</span><span class="sxs-lookup"><span data-stu-id="d3dba-127">options</span></span>|<span data-ttu-id="d3dba-128">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d3dba-128">WorksheetProtectionOptions</span></span>|<span data-ttu-id="d3dba-p104">Optional. Optionen für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="d3dba-p104">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d3dba-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3dba-131">Response</span></span>

<span data-ttu-id="d3dba-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3dba-p105">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3dba-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3dba-134">Example</span></span>
<span data-ttu-id="d3dba-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d3dba-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3dba-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3dba-136">Request</span></span>
<span data-ttu-id="d3dba-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3dba-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d3dba-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3dba-138">Response</span></span>
<span data-ttu-id="d3dba-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3dba-139">Here is an example of the response.</span></span> 
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
