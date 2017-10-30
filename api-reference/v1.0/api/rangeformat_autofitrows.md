# <a name="rangeformat-autofitrows"></a><span data-ttu-id="8b922-101">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="8b922-101">RangeFormat: autofitRows</span></span>

<span data-ttu-id="8b922-102">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="8b922-102">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b922-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b922-103">Permissions</span></span>
<span data-ttu-id="8b922-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b922-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b922-106">Permission type</span></span>      | <span data-ttu-id="8b922-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b922-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b922-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b922-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8b922-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b922-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b922-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b922-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b922-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b922-111">Not supported.</span></span>    |
|<span data-ttu-id="8b922-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b922-112">Application</span></span> | <span data-ttu-id="8b922-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b922-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b922-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b922-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="8b922-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b922-115">Request headers</span></span>
| <span data-ttu-id="8b922-116">Name</span><span class="sxs-lookup"><span data-stu-id="8b922-116">Name</span></span>       | <span data-ttu-id="8b922-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b922-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b922-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b922-118">Authorization</span></span>  | <span data-ttu-id="8b922-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b922-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b922-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b922-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8b922-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b922-122">Response</span></span>

<span data-ttu-id="8b922-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b922-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b922-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b922-125">Example</span></span>
<span data-ttu-id="8b922-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8b922-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b922-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b922-127">Request</span></span>
<span data-ttu-id="8b922-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b922-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="8b922-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b922-129">Response</span></span>
<span data-ttu-id="8b922-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b922-130">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->