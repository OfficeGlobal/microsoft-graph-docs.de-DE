# <a name="delete-device"></a><span data-ttu-id="1194f-101">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="1194f-101">Delete device</span></span>

<span data-ttu-id="1194f-102">Mit dieser API können Sie registrierte Geräte löschen.</span><span class="sxs-lookup"><span data-stu-id="1194f-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1194f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1194f-103">Permissions</span></span>
<span data-ttu-id="1194f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1194f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1194f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1194f-106">Permission type</span></span>      | <span data-ttu-id="1194f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1194f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1194f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1194f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1194f-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1194f-109">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1194f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1194f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1194f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1194f-111">Not supported.</span></span>    |
|<span data-ttu-id="1194f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1194f-112">Application</span></span> | <span data-ttu-id="1194f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1194f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1194f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1194f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="1194f-115">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="1194f-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1194f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1194f-116">Request headers</span></span>
| <span data-ttu-id="1194f-117">Name</span><span class="sxs-lookup"><span data-stu-id="1194f-117">Name</span></span>       | <span data-ttu-id="1194f-118">Typ</span><span class="sxs-lookup"><span data-stu-id="1194f-118">Type</span></span> | <span data-ttu-id="1194f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1194f-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1194f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1194f-120">Authorization</span></span>  | <span data-ttu-id="1194f-121">string</span><span class="sxs-lookup"><span data-stu-id="1194f-121">string</span></span>  | <span data-ttu-id="1194f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1194f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1194f-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1194f-124">Request body</span></span>
<span data-ttu-id="1194f-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1194f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1194f-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="1194f-126">Response</span></span>

<span data-ttu-id="1194f-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1194f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1194f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1194f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1194f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1194f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="1194f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1194f-131">Response</span></span>

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
