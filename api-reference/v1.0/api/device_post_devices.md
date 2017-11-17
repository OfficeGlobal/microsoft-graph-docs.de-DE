# <a name="create-device"></a><span data-ttu-id="304ac-101">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="304ac-101">Create device</span></span>

<span data-ttu-id="304ac-102">Mit dieser API können Sie ein neues Gerät in der Organisation registrieren.</span><span class="sxs-lookup"><span data-stu-id="304ac-102">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="304ac-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="304ac-103">Permissions</span></span>
<span data-ttu-id="304ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="304ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="304ac-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="304ac-106">Permission type</span></span>      | <span data-ttu-id="304ac-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="304ac-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="304ac-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="304ac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="304ac-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="304ac-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="304ac-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="304ac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304ac-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="304ac-111">Not supported.</span></span>    |
|<span data-ttu-id="304ac-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="304ac-112">Application</span></span> | <span data-ttu-id="304ac-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304ac-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="304ac-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="304ac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="304ac-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="304ac-115">Request headers</span></span>
| <span data-ttu-id="304ac-116">Name</span><span class="sxs-lookup"><span data-stu-id="304ac-116">Name</span></span>       | <span data-ttu-id="304ac-117">Typ</span><span class="sxs-lookup"><span data-stu-id="304ac-117">Type</span></span> | <span data-ttu-id="304ac-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="304ac-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="304ac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="304ac-119">Authorization</span></span>  | <span data-ttu-id="304ac-120">string</span><span class="sxs-lookup"><span data-stu-id="304ac-120">string</span></span>  | <span data-ttu-id="304ac-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="304ac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="304ac-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="304ac-123">Content-type</span></span> | <span data-ttu-id="304ac-124">string</span><span class="sxs-lookup"><span data-stu-id="304ac-124">string</span></span> | <span data-ttu-id="304ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="304ac-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="304ac-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="304ac-126">Request body</span></span>
<span data-ttu-id="304ac-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="304ac-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="304ac-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="304ac-128">Response</span></span>

<span data-ttu-id="304ac-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="304ac-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304ac-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="304ac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="304ac-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="304ac-131">Request</span></span>
<span data-ttu-id="304ac-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="304ac-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
<span data-ttu-id="304ac-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="304ac-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="304ac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="304ac-134">Response</span></span>
<span data-ttu-id="304ac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="304ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
