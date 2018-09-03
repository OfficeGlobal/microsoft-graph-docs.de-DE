# <a name="create-table"></a><span data-ttu-id="f8dc0-101">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="f8dc0-101">Create table</span></span>

<span data-ttu-id="f8dc0-102">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8dc0-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8dc0-103">Permissions</span></span>
<span data-ttu-id="f8dc0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8dc0-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8dc0-106">Permission type</span></span>      | <span data-ttu-id="f8dc0-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8dc0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8dc0-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8dc0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f8dc0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8dc0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8dc0-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8dc0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8dc0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8dc0-111">Not supported.</span></span>    |
|<span data-ttu-id="f8dc0-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-112">Application</span></span> | <span data-ttu-id="f8dc0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8dc0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8dc0-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="f8dc0-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8dc0-115">Request headers</span></span>
| <span data-ttu-id="f8dc0-116">Name</span><span class="sxs-lookup"><span data-stu-id="f8dc0-116">Name</span></span>       | <span data-ttu-id="f8dc0-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8dc0-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-118">Authorization</span></span>  | <span data-ttu-id="f8dc0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8dc0-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f8dc0-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8dc0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8dc0-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8dc0-124">Request body</span></span>
<span data-ttu-id="f8dc0-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8dc0-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="f8dc0-126">Parameter</span></span>           | <span data-ttu-id="f8dc0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f8dc0-127">Type</span></span>      |<span data-ttu-id="f8dc0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-128">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="f8dc0-129">Adresse</span><span class="sxs-lookup"><span data-stu-id="f8dc0-129">Address</span></span>  | <span data-ttu-id="f8dc0-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8dc0-130">string</span></span>| <span data-ttu-id="f8dc0-p104">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="f8dc0-134">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f8dc0-134">hasHeaders</span></span>  | <span data-ttu-id="f8dc0-135">boolesch</span><span class="sxs-lookup"><span data-stu-id="f8dc0-135">boolean</span></span>|<span data-ttu-id="f8dc0-p105">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="f8dc0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8dc0-139">Response</span></span>

<span data-ttu-id="f8dc0-140">Wenn erfolgreich, gibt diese Methode einen Antwortcode `201 Created` und ein [WorkbookTable](../resources/table.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-140">If successful, this method returns `201 Created` response code and [groupSetting](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8dc0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8dc0-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8dc0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8dc0-142">Request</span></span>
<span data-ttu-id="f8dc0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f8dc0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8dc0-144">Response</span></span>
<span data-ttu-id="f8dc0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8dc0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
