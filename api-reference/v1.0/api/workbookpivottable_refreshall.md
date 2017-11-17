# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="3de3e-101">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="3de3e-101">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="3de3e-102">Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="3de3e-102">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="3de3e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3de3e-103">Permissions</span></span>
<span data-ttu-id="3de3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3de3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3de3e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3de3e-106">Permission type</span></span>      | <span data-ttu-id="3de3e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3de3e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3de3e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3de3e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3de3e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de3e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3de3e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3de3e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3de3e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3de3e-111">Not supported.</span></span>    |
|<span data-ttu-id="3de3e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3de3e-112">Application</span></span> | <span data-ttu-id="3de3e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3de3e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3de3e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3de3e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="3de3e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3de3e-115">Request headers</span></span>
| <span data-ttu-id="3de3e-116">Name</span><span class="sxs-lookup"><span data-stu-id="3de3e-116">Name</span></span>       | <span data-ttu-id="3de3e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3de3e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3de3e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="3de3e-118">Authorization</span></span>  | <span data-ttu-id="3de3e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3de3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3de3e-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3de3e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3de3e-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3de3e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de3e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3de3e-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="3de3e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="3de3e-125">Response</span></span>
<span data-ttu-id="3de3e-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3de3e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de3e-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3de3e-128">Example</span></span>
<span data-ttu-id="3de3e-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3de3e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3de3e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3de3e-130">Request</span></span>
<span data-ttu-id="3de3e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3de3e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="3de3e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3de3e-132">Response</span></span>
<span data-ttu-id="3de3e-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3de3e-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
