# <a name="tablerow-delete"></a><span data-ttu-id="2af58-101">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="2af58-101">TableRow: delete</span></span>

<span data-ttu-id="2af58-102">Löscht die Zeile aus der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="2af58-102">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2af58-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2af58-103">Permissions</span></span>
<span data-ttu-id="2af58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2af58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2af58-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2af58-106">Permission type</span></span>      | <span data-ttu-id="2af58-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2af58-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2af58-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2af58-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2af58-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2af58-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2af58-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2af58-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2af58-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2af58-111">Not supported.</span></span>    |
|<span data-ttu-id="2af58-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2af58-112">Application</span></span> | <span data-ttu-id="2af58-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2af58-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2af58-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2af58-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="2af58-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2af58-115">Request headers</span></span>
| <span data-ttu-id="2af58-116">Name</span><span class="sxs-lookup"><span data-stu-id="2af58-116">Name</span></span>       | <span data-ttu-id="2af58-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2af58-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2af58-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af58-118">Authorization</span></span>  | <span data-ttu-id="2af58-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2af58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2af58-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2af58-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2af58-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="2af58-122">Response</span></span>

<span data-ttu-id="2af58-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2af58-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af58-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2af58-125">Example</span></span>
<span data-ttu-id="2af58-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2af58-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2af58-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2af58-127">Request</span></span>
<span data-ttu-id="2af58-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2af58-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="2af58-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2af58-129">Response</span></span>
<span data-ttu-id="2af58-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2af58-130">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->