# <a name="create-table"></a><span data-ttu-id="4fcb5-101">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="4fcb5-101">Create Table</span></span>

<span data-ttu-id="4fcb5-102">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fcb5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4fcb5-103">Permissions</span></span>
<span data-ttu-id="4fcb5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fcb5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4fcb5-106">Permission type</span></span>      | <span data-ttu-id="4fcb5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4fcb5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fcb5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4fcb5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4fcb5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fcb5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4fcb5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4fcb5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fcb5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fcb5-111">Not supported.</span></span>    |
|<span data-ttu-id="4fcb5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-112">Application</span></span> | <span data-ttu-id="4fcb5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fcb5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fcb5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{table-id}/add

```
## <a name="request-headers"></a><span data-ttu-id="4fcb5-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4fcb5-115">Request headers</span></span>
| <span data-ttu-id="4fcb5-116">Name</span><span class="sxs-lookup"><span data-stu-id="4fcb5-116">Name</span></span>       | <span data-ttu-id="4fcb5-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4fcb5-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-118">Authorization</span></span>  | <span data-ttu-id="4fcb5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fcb5-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4fcb5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4fcb5-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

### <a name="request-parameters"></a><span data-ttu-id="4fcb5-124">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="4fcb5-124">Request parameters</span></span>
| <span data-ttu-id="4fcb5-125">Name</span><span class="sxs-lookup"><span data-stu-id="4fcb5-125">Name</span></span>           | <span data-ttu-id="4fcb5-126">Typ</span><span class="sxs-lookup"><span data-stu-id="4fcb5-126">Type</span></span>      |<span data-ttu-id="4fcb5-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-127">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="4fcb5-128">Address</span><span class="sxs-lookup"><span data-stu-id="4fcb5-128">Address</span></span>  | <span data-ttu-id="4fcb5-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4fcb5-129">string</span></span>| <span data-ttu-id="4fcb5-p104">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="4fcb5-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="4fcb5-133">hasHeaders</span></span>  | <span data-ttu-id="4fcb5-134">boolesch</span><span class="sxs-lookup"><span data-stu-id="4fcb5-134">boolean</span></span>|<span data-ttu-id="4fcb5-p105">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="4fcb5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fcb5-138">Response</span></span>

<span data-ttu-id="4fcb5-139">Wenn erfolgreich, gibt diese Methode einen Antwortcode `201 Created` und ein [WorkbookTable](../resources/table.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-139">If successful, this method returns `201 Created` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fcb5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4fcb5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fcb5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fcb5-141">Request</span></span>
<span data-ttu-id="4fcb5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{table-id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="4fcb5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fcb5-143">Response</span></span>
<span data-ttu-id="4fcb5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4fcb5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
