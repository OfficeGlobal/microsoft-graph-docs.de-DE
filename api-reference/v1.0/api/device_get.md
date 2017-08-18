# <a name="get-device"></a><span data-ttu-id="59a3e-101">Gerät abrufen</span><span class="sxs-lookup"><span data-stu-id="59a3e-101">Get device</span></span>

<span data-ttu-id="59a3e-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Geräteobjekts.</span><span class="sxs-lookup"><span data-stu-id="59a3e-102">Get the properties and relationships of a device object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59a3e-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="59a3e-103">Prerequisites</span></span>
<span data-ttu-id="59a3e-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Device.ReadWrite.All* oder *Directory.Read.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="59a3e-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="59a3e-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59a3e-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="59a3e-106">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="59a3e-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="59a3e-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="59a3e-107">Optional query parameters</span></span>
<span data-ttu-id="59a3e-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59a3e-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59a3e-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59a3e-109">Request headers</span></span>
| <span data-ttu-id="59a3e-110">Name</span><span class="sxs-lookup"><span data-stu-id="59a3e-110">Name</span></span>       | <span data-ttu-id="59a3e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="59a3e-111">Type</span></span> | <span data-ttu-id="59a3e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59a3e-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59a3e-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="59a3e-113">Authorization</span></span>  | <span data-ttu-id="59a3e-114">string</span><span class="sxs-lookup"><span data-stu-id="59a3e-114">string</span></span>  | <span data-ttu-id="59a3e-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59a3e-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59a3e-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59a3e-117">Request body</span></span>
<span data-ttu-id="59a3e-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="59a3e-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59a3e-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="59a3e-119">Response</span></span>

<span data-ttu-id="59a3e-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59a3e-120">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59a3e-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59a3e-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59a3e-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59a3e-122">Request</span></span>
<span data-ttu-id="59a3e-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59a3e-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="59a3e-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="59a3e-124">Response</span></span>
<span data-ttu-id="59a3e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59a3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
