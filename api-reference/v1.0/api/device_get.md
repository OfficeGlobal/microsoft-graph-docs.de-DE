# <a name="get-device"></a><span data-ttu-id="45cf9-101">Gerät abrufen</span><span class="sxs-lookup"><span data-stu-id="45cf9-101">Get device</span></span>

<span data-ttu-id="45cf9-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="45cf9-102">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="45cf9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45cf9-103">Permissions</span></span>
<span data-ttu-id="45cf9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="45cf9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45cf9-106">Permission type</span></span>      | <span data-ttu-id="45cf9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45cf9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45cf9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45cf9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="45cf9-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45cf9-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45cf9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45cf9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45cf9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45cf9-111">Not supported.</span></span>    |
|<span data-ttu-id="45cf9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45cf9-112">Application</span></span> | <span data-ttu-id="45cf9-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45cf9-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45cf9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45cf9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="45cf9-115">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="45cf9-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="45cf9-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45cf9-116">Optional query parameters</span></span>
<span data-ttu-id="45cf9-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45cf9-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45cf9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45cf9-118">Request headers</span></span>
| <span data-ttu-id="45cf9-119">Name</span><span class="sxs-lookup"><span data-stu-id="45cf9-119">Name</span></span>       | <span data-ttu-id="45cf9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="45cf9-120">Type</span></span> | <span data-ttu-id="45cf9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45cf9-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45cf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45cf9-122">Authorization</span></span>  | <span data-ttu-id="45cf9-123">string</span><span class="sxs-lookup"><span data-stu-id="45cf9-123">string</span></span>  | <span data-ttu-id="45cf9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45cf9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45cf9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45cf9-126">Request body</span></span>
<span data-ttu-id="45cf9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45cf9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45cf9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="45cf9-128">Response</span></span>

<span data-ttu-id="45cf9-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45cf9-129">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45cf9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45cf9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45cf9-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45cf9-131">Request</span></span>
<span data-ttu-id="45cf9-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45cf9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="45cf9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="45cf9-133">Response</span></span>
<span data-ttu-id="45cf9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45cf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
