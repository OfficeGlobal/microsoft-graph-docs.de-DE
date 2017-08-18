# <a name="delete-device"></a><span data-ttu-id="aa195-101">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="aa195-101">Delete device</span></span>

<span data-ttu-id="aa195-102">Dient zum Löschen eines registrierten Geräts.</span><span class="sxs-lookup"><span data-stu-id="aa195-102">Delete a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa195-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aa195-103">Prerequisites</span></span>
<span data-ttu-id="aa195-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="aa195-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="aa195-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa195-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="aa195-106">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="aa195-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa195-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa195-107">Request headers</span></span>
| <span data-ttu-id="aa195-108">Name</span><span class="sxs-lookup"><span data-stu-id="aa195-108">Name</span></span>       | <span data-ttu-id="aa195-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aa195-109">Type</span></span> | <span data-ttu-id="aa195-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa195-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa195-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa195-111">Authorization</span></span>  | <span data-ttu-id="aa195-112">string</span><span class="sxs-lookup"><span data-stu-id="aa195-112">string</span></span>  | <span data-ttu-id="aa195-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa195-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa195-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa195-115">Request body</span></span>
<span data-ttu-id="aa195-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa195-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa195-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa195-117">Response</span></span>

<span data-ttu-id="aa195-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa195-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa195-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa195-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa195-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa195-121">Request</span></span>
<span data-ttu-id="aa195-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa195-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="aa195-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa195-123">Response</span></span>
<span data-ttu-id="aa195-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa195-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
