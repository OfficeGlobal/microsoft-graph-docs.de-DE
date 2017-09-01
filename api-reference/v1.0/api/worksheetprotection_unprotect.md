# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="295a1-101">WorksheetProtection: Schutz aufheben</span><span class="sxs-lookup"><span data-stu-id="295a1-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="295a1-102">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="295a1-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="295a1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="295a1-103">Permissions</span></span>
<span data-ttu-id="295a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="295a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="295a1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="295a1-106">Permission type</span></span>      | <span data-ttu-id="295a1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="295a1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="295a1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="295a1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="295a1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="295a1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="295a1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="295a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="295a1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="295a1-111">Not supported.</span></span>    |
|<span data-ttu-id="295a1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="295a1-112">Application</span></span> | <span data-ttu-id="295a1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="295a1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="295a1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="295a1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="295a1-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="295a1-115">Request headers</span></span>
| <span data-ttu-id="295a1-116">Name</span><span class="sxs-lookup"><span data-stu-id="295a1-116">Name</span></span>       | <span data-ttu-id="295a1-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="295a1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="295a1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="295a1-118">Authorization</span></span>  | <span data-ttu-id="295a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="295a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="295a1-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="295a1-121">Request body</span></span>
<span data-ttu-id="295a1-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="295a1-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="295a1-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="295a1-123">Parameter</span></span>    | <span data-ttu-id="295a1-124">Typ</span><span class="sxs-lookup"><span data-stu-id="295a1-124">Type</span></span>   |<span data-ttu-id="295a1-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="295a1-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="295a1-126">password</span><span class="sxs-lookup"><span data-stu-id="295a1-126">password</span></span>|<span data-ttu-id="295a1-127">string</span><span class="sxs-lookup"><span data-stu-id="295a1-127">string</span></span>|<span data-ttu-id="295a1-p103">Optional. Kennwort für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="295a1-p103">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="295a1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="295a1-130">Response</span></span>

<span data-ttu-id="295a1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="295a1-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="295a1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="295a1-133">Example</span></span>
<span data-ttu-id="295a1-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="295a1-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="295a1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="295a1-135">Request</span></span>
<span data-ttu-id="295a1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="295a1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="295a1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="295a1-137">Response</span></span>
<span data-ttu-id="295a1-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="295a1-138">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->