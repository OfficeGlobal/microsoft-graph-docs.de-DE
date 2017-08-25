# <a name="list-devices"></a><span data-ttu-id="742a1-101">Geräte auflisten</span><span class="sxs-lookup"><span data-stu-id="742a1-101">List devices</span></span>

<span data-ttu-id="742a1-102">Mit dieser API können Sie eine Liste der in einer Organisation registrierten Geräteobjekte abrufen.</span><span class="sxs-lookup"><span data-stu-id="742a1-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="742a1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="742a1-103">Permissions</span></span>
<span data-ttu-id="742a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="742a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="742a1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="742a1-106">Permission type</span></span>      | <span data-ttu-id="742a1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="742a1-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="742a1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="742a1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="742a1-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="742a1-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="742a1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="742a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="742a1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="742a1-111">Not supported.</span></span>    | 
|<span data-ttu-id="742a1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="742a1-112">Application</span></span> | <span data-ttu-id="742a1-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="742a1-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="742a1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="742a1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="742a1-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="742a1-115">Optional query parameters</span></span>
<span data-ttu-id="742a1-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="742a1-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="742a1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="742a1-117">Request headers</span></span>
| <span data-ttu-id="742a1-118">Name</span><span class="sxs-lookup"><span data-stu-id="742a1-118">Name</span></span>       | <span data-ttu-id="742a1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="742a1-119">Type</span></span> | <span data-ttu-id="742a1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="742a1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="742a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="742a1-121">Authorization</span></span>  | <span data-ttu-id="742a1-122">string</span><span class="sxs-lookup"><span data-stu-id="742a1-122">string</span></span>  | <span data-ttu-id="742a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="742a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="742a1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="742a1-125">Request body</span></span>
<span data-ttu-id="742a1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="742a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="742a1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="742a1-127">Response</span></span>

<span data-ttu-id="742a1-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [device](../resources/device.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="742a1-128">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="742a1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="742a1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="742a1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="742a1-130">Request</span></span>
<span data-ttu-id="742a1-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="742a1-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="742a1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="742a1-132">Response</span></span>
<span data-ttu-id="742a1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="742a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "alternativeSecurityIds":
      [
        {
          "type":2,
          "key":"Y3YxN2E1MWFlYw==",
          "identityProvider": null
        }
      ],
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
