# <a name="get-directoryrole"></a><span data-ttu-id="3b35f-101">directoryRole abrufen</span><span class="sxs-lookup"><span data-stu-id="3b35f-101">Get directoryRole</span></span>

<span data-ttu-id="3b35f-102">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „directoryRole“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="3b35f-102">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b35f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b35f-103">Permissions</span></span>
<span data-ttu-id="3b35f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b35f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b35f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b35f-106">Permission type</span></span>      | <span data-ttu-id="3b35f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b35f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3b35f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b35f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3b35f-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b35f-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="3b35f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b35f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b35f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b35f-111">Not supported.</span></span>    | 
|<span data-ttu-id="3b35f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b35f-112">Application</span></span> | <span data-ttu-id="3b35f-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b35f-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b35f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b35f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b35f-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b35f-115">Optional query parameters</span></span>
<span data-ttu-id="3b35f-116">Die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="3b35f-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b35f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b35f-117">Request headers</span></span>
| <span data-ttu-id="3b35f-118">Name</span><span class="sxs-lookup"><span data-stu-id="3b35f-118">Name</span></span>       | <span data-ttu-id="3b35f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="3b35f-119">Type</span></span> | <span data-ttu-id="3b35f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b35f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b35f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b35f-121">Authorization</span></span>  | <span data-ttu-id="3b35f-122">string</span><span class="sxs-lookup"><span data-stu-id="3b35f-122">string</span></span>  | <span data-ttu-id="3b35f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b35f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b35f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b35f-125">Request body</span></span>
<span data-ttu-id="3b35f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b35f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b35f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b35f-127">Response</span></span>

<span data-ttu-id="3b35f-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b35f-128">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b35f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b35f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b35f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b35f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="3b35f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b35f-131">Response</span></span>
<span data-ttu-id="3b35f-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b35f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
