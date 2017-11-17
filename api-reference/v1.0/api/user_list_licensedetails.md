# <a name="list-licensedetails"></a><span data-ttu-id="e544c-101">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="e544c-101">List licenseDetails</span></span>

<span data-ttu-id="e544c-102">Mit dieser API können Sie eine Liste von Objekten des Typs „licenseDetails“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="e544c-102">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e544c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e544c-103">Permissions</span></span>
<span data-ttu-id="e544c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e544c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e544c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e544c-106">Permission type</span></span>      | <span data-ttu-id="e544c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e544c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e544c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e544c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e544c-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e544c-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e544c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e544c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e544c-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="e544c-111">User.Read</span></span>    |
|<span data-ttu-id="e544c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e544c-112">Application</span></span> | <span data-ttu-id="e544c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e544c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e544c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e544c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e544c-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e544c-115">Optional query parameters</span></span>
<span data-ttu-id="e544c-116">Diese Methode bietet **keine** Unterstützung für [OData Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="e544c-116">This method does **not** support [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e544c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e544c-117">Request headers</span></span>
| <span data-ttu-id="e544c-118">Name</span><span class="sxs-lookup"><span data-stu-id="e544c-118">Name</span></span>      |<span data-ttu-id="e544c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e544c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e544c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e544c-120">Authorization</span></span>  | <span data-ttu-id="e544c-121">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="e544c-121">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="e544c-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e544c-122">Request body</span></span>
<span data-ttu-id="e544c-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e544c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e544c-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="e544c-124">Response</span></span>

<span data-ttu-id="e544c-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [licenseDetails](../resources/licensedetails.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e544c-125">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e544c-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e544c-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e544c-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e544c-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="e544c-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e544c-128">Response</span></span>
<span data-ttu-id="e544c-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e544c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->