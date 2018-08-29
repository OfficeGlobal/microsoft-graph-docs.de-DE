# <a name="table-reapplyfilters"></a><span data-ttu-id="892ab-101">Tabelle: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="892ab-101">Table: reapplyFilters</span></span>

<span data-ttu-id="892ab-102">Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="892ab-102">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="892ab-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="892ab-103">Permissions</span></span>
<span data-ttu-id="892ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="892ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="892ab-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="892ab-106">Permission type</span></span>      | <span data-ttu-id="892ab-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="892ab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="892ab-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="892ab-108">Delegated (work or school account)</span></span> | <span data-ttu-id="892ab-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892ab-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892ab-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="892ab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892ab-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="892ab-111">Not supported.</span></span>    |
|<span data-ttu-id="892ab-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="892ab-112">Application</span></span> | <span data-ttu-id="892ab-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="892ab-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="892ab-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="892ab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="892ab-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="892ab-115">Request headers</span></span>
| <span data-ttu-id="892ab-116">Name</span><span class="sxs-lookup"><span data-stu-id="892ab-116">Name</span></span>       | <span data-ttu-id="892ab-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="892ab-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="892ab-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="892ab-118">Authorization</span></span>  | <span data-ttu-id="892ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="892ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="892ab-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="892ab-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="892ab-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="892ab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="892ab-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="892ab-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="892ab-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="892ab-125">Response</span></span>

<span data-ttu-id="892ab-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="892ab-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892ab-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="892ab-128">Example</span></span>
<span data-ttu-id="892ab-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="892ab-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="892ab-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="892ab-130">Request</span></span>
<span data-ttu-id="892ab-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="892ab-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="892ab-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="892ab-132">Response</span></span>
<span data-ttu-id="892ab-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="892ab-133">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->