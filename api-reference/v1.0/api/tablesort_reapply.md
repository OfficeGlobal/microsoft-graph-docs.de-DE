# <a name="tablesort-reapply"></a><span data-ttu-id="498e9-101">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="498e9-101">TableSort: reapply</span></span>

<span data-ttu-id="498e9-102">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="498e9-102">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="498e9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="498e9-103">Permissions</span></span>
<span data-ttu-id="498e9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="498e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="498e9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="498e9-106">Permission type</span></span>      | <span data-ttu-id="498e9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="498e9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="498e9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="498e9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="498e9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="498e9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="498e9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="498e9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="498e9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="498e9-111">Not supported.</span></span>    |
|<span data-ttu-id="498e9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="498e9-112">Application</span></span> | <span data-ttu-id="498e9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="498e9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="498e9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="498e9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="498e9-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="498e9-115">Request headers</span></span>
| <span data-ttu-id="498e9-116">Name</span><span class="sxs-lookup"><span data-stu-id="498e9-116">Name</span></span>       | <span data-ttu-id="498e9-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="498e9-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="498e9-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="498e9-118">Authorization</span></span>  | <span data-ttu-id="498e9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="498e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="498e9-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="498e9-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="498e9-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="498e9-122">Response</span></span>

<span data-ttu-id="498e9-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="498e9-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="498e9-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="498e9-125">Example</span></span>
<span data-ttu-id="498e9-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="498e9-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="498e9-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="498e9-127">Request</span></span>
<span data-ttu-id="498e9-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="498e9-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="498e9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="498e9-129">Response</span></span>
<span data-ttu-id="498e9-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="498e9-130">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->