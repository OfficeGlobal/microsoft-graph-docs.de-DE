# <a name="chartfill-clear"></a><span data-ttu-id="0298b-101">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="0298b-101">ChartFill: clear</span></span>

<span data-ttu-id="0298b-102">Dient zum Löschen der Füllfarbe eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="0298b-102">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="0298b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0298b-103">Permissions</span></span>
<span data-ttu-id="0298b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0298b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0298b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0298b-106">Permission type</span></span>      | <span data-ttu-id="0298b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0298b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0298b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0298b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0298b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0298b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0298b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0298b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0298b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0298b-111">Not supported.</span></span>    |
|<span data-ttu-id="0298b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0298b-112">Application</span></span> | <span data-ttu-id="0298b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0298b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0298b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0298b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="0298b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0298b-115">Request headers</span></span>
| <span data-ttu-id="0298b-116">Name</span><span class="sxs-lookup"><span data-stu-id="0298b-116">Name</span></span>       | <span data-ttu-id="0298b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0298b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0298b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0298b-118">Authorization</span></span>  | <span data-ttu-id="0298b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0298b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0298b-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0298b-121">Request body</span></span>
<span data-ttu-id="0298b-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0298b-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0298b-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="0298b-123">Response</span></span>

<span data-ttu-id="0298b-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0298b-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0298b-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0298b-126">Example</span></span>
<span data-ttu-id="0298b-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0298b-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0298b-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0298b-128">Request</span></span>
<span data-ttu-id="0298b-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0298b-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="0298b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0298b-130">Response</span></span>
<span data-ttu-id="0298b-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0298b-131">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->