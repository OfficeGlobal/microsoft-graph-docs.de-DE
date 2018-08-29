# <a name="tablesort-clear"></a><span data-ttu-id="8b2a2-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="8b2a2-101">TableSort: clear</span></span>

<span data-ttu-id="8b2a2-p101">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b2a2-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b2a2-104">Permissions</span></span>
<span data-ttu-id="8b2a2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b2a2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b2a2-107">Permission type</span></span>      | <span data-ttu-id="8b2a2-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b2a2-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b2a2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b2a2-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2a2-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2a2-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b2a2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b2a2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2a2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b2a2-112">Not supported.</span></span>    |
|<span data-ttu-id="8b2a2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b2a2-113">Application</span></span> | <span data-ttu-id="8b2a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b2a2-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b2a2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2a2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="8b2a2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b2a2-116">Request headers</span></span>
| <span data-ttu-id="8b2a2-117">Name</span><span class="sxs-lookup"><span data-stu-id="8b2a2-117">Name</span></span>       | <span data-ttu-id="8b2a2-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b2a2-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b2a2-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8b2a2-119">Authorization</span></span>  | <span data-ttu-id="8b2a2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b2a2-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8b2a2-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b2a2-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b2a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b2a2-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8b2a2-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2a2-126">Response</span></span>

<span data-ttu-id="8b2a2-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2a2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b2a2-129">Example</span></span>
<span data-ttu-id="8b2a2-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b2a2-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2a2-131">Request</span></span>
<span data-ttu-id="8b2a2-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="8b2a2-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2a2-133">Response</span></span>
<span data-ttu-id="8b2a2-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b2a2-134">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->