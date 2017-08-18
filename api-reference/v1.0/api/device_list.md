# <a name="list-devices"></a><span data-ttu-id="1f280-101">Geräte auflisten</span><span class="sxs-lookup"><span data-stu-id="1f280-101">List devices</span></span>

<span data-ttu-id="1f280-102">Dient zum Abrufen einer Liste von Geräteobjekten, die in der Organisation registriert sind.</span><span class="sxs-lookup"><span data-stu-id="1f280-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f280-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="1f280-103">Prerequisites</span></span>
<span data-ttu-id="1f280-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Device.ReadWrite.All* oder *Directory.Read.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="1f280-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="1f280-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f280-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f280-106">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f280-106">Optional query parameters</span></span>
<span data-ttu-id="1f280-107">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f280-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f280-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f280-108">Request headers</span></span>
| <span data-ttu-id="1f280-109">Name</span><span class="sxs-lookup"><span data-stu-id="1f280-109">Name</span></span>       | <span data-ttu-id="1f280-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1f280-110">Type</span></span> | <span data-ttu-id="1f280-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f280-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f280-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f280-112">Authorization</span></span>  | <span data-ttu-id="1f280-113">string</span><span class="sxs-lookup"><span data-stu-id="1f280-113">string</span></span>  | <span data-ttu-id="1f280-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f280-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f280-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f280-116">Request body</span></span>
<span data-ttu-id="1f280-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f280-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f280-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f280-118">Response</span></span>

<span data-ttu-id="1f280-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [device](../resources/device.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f280-119">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f280-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f280-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f280-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f280-121">Request</span></span>
<span data-ttu-id="1f280-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f280-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="1f280-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f280-123">Response</span></span>
<span data-ttu-id="1f280-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f280-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
