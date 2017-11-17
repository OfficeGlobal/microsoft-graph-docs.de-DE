# <a name="update-device"></a><span data-ttu-id="9d67d-101">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9d67d-101">Update device</span></span>

<span data-ttu-id="9d67d-102">Mit dieser API können Sie die Eigenschaften eines registrierten Geräts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9d67d-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d67d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d67d-103">Permissions</span></span>
<span data-ttu-id="9d67d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d67d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9d67d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d67d-106">Permission type</span></span>      | <span data-ttu-id="9d67d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d67d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d67d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d67d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d67d-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d67d-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d67d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d67d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d67d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d67d-111">Not supported.</span></span>    |
|<span data-ttu-id="9d67d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d67d-112">Application</span></span> | <span data-ttu-id="9d67d-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d67d-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d67d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d67d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="9d67d-115">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="9d67d-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d67d-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d67d-116">Request headers</span></span>
| <span data-ttu-id="9d67d-117">Name</span><span class="sxs-lookup"><span data-stu-id="9d67d-117">Name</span></span>       | <span data-ttu-id="9d67d-118">Typ</span><span class="sxs-lookup"><span data-stu-id="9d67d-118">Type</span></span> | <span data-ttu-id="9d67d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d67d-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d67d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d67d-120">Authorization</span></span>  | <span data-ttu-id="9d67d-121">string</span><span class="sxs-lookup"><span data-stu-id="9d67d-121">string</span></span>  | <span data-ttu-id="9d67d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d67d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d67d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d67d-124">Request body</span></span>
<span data-ttu-id="9d67d-125">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9d67d-125">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="9d67d-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d67d-126">Response</span></span>

<span data-ttu-id="9d67d-127">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d67d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d67d-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d67d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d67d-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d67d-129">Request</span></span>
<span data-ttu-id="9d67d-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d67d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="9d67d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d67d-131">Response</span></span>
<span data-ttu-id="9d67d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d67d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
