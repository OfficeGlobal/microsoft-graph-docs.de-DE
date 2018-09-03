# <a name="create-table"></a><span data-ttu-id="b14d5-101">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="b14d5-101">Create Table</span></span>

<span data-ttu-id="b14d5-102">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="b14d5-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="b14d5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b14d5-103">Permissions</span></span>
<span data-ttu-id="b14d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b14d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b14d5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b14d5-106">Permission type</span></span>      | <span data-ttu-id="b14d5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b14d5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b14d5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b14d5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b14d5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b14d5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b14d5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b14d5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b14d5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b14d5-111">Not supported.</span></span>    |
|<span data-ttu-id="b14d5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b14d5-112">Application</span></span> | <span data-ttu-id="b14d5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b14d5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b14d5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b14d5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="b14d5-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b14d5-115">Request headers</span></span>
| <span data-ttu-id="b14d5-116">Name</span><span class="sxs-lookup"><span data-stu-id="b14d5-116">Name</span></span>       | <span data-ttu-id="b14d5-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b14d5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b14d5-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b14d5-118">Authorization</span></span>  | <span data-ttu-id="b14d5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b14d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b14d5-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b14d5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b14d5-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b14d5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b14d5-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b14d5-124">Request body</span></span>
<span data-ttu-id="b14d5-125">Geben Sie im Anforderungstext die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b14d5-125">In the request body, supply following parameters.</span></span> 

### <a name="request-parameters"></a><span data-ttu-id="b14d5-126">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="b14d5-126">Request parameters</span></span>
| <span data-ttu-id="b14d5-127">Name</span><span class="sxs-lookup"><span data-stu-id="b14d5-127">Name</span></span>           | <span data-ttu-id="b14d5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b14d5-128">Type</span></span>      |<span data-ttu-id="b14d5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b14d5-129">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="b14d5-130">Address</span><span class="sxs-lookup"><span data-stu-id="b14d5-130">Address</span></span>  | <span data-ttu-id="b14d5-131">string</span><span class="sxs-lookup"><span data-stu-id="b14d5-131">string</span></span>| <span data-ttu-id="b14d5-p104">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="b14d5-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="b14d5-135">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b14d5-135">hasHeaders</span></span>  | <span data-ttu-id="b14d5-136">boolean</span><span class="sxs-lookup"><span data-stu-id="b14d5-136">boolean</span></span>|<span data-ttu-id="b14d5-p105">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="b14d5-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="b14d5-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b14d5-140">Response</span></span>

<span data-ttu-id="b14d5-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [WorkbookTable](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b14d5-141">If successful, this method returns `201 Created` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b14d5-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b14d5-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b14d5-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b14d5-143">Request</span></span>
<span data-ttu-id="b14d5-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b14d5-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="b14d5-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b14d5-145">Response</span></span>
<span data-ttu-id="b14d5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b14d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
