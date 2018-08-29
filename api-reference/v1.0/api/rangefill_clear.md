# <a name="rangefill-clear"></a><span data-ttu-id="195d6-101">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="195d6-101">RangeFill: clear</span></span>

<span data-ttu-id="195d6-102">Setzt den Hintergrund des Bereichs zurück.</span><span class="sxs-lookup"><span data-stu-id="195d6-102">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="195d6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="195d6-103">Permissions</span></span>
<span data-ttu-id="195d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="195d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="195d6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="195d6-106">Permission type</span></span>      | <span data-ttu-id="195d6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="195d6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="195d6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="195d6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="195d6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="195d6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="195d6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="195d6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="195d6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="195d6-111">Not supported.</span></span>    |
|<span data-ttu-id="195d6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="195d6-112">Application</span></span> | <span data-ttu-id="195d6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="195d6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="195d6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="195d6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/fill/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="195d6-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="195d6-115">Request headers</span></span>
| <span data-ttu-id="195d6-116">Name</span><span class="sxs-lookup"><span data-stu-id="195d6-116">Name</span></span>       | <span data-ttu-id="195d6-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="195d6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="195d6-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="195d6-118">Authorization</span></span>  | <span data-ttu-id="195d6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="195d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="195d6-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="195d6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="195d6-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="195d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="195d6-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="195d6-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="195d6-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="195d6-125">Response</span></span>

<span data-ttu-id="195d6-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="195d6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="195d6-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="195d6-128">Example</span></span>
<span data-ttu-id="195d6-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="195d6-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="195d6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="195d6-130">Request</span></span>
<span data-ttu-id="195d6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="195d6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="195d6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="195d6-132">Response</span></span>
<span data-ttu-id="195d6-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="195d6-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->