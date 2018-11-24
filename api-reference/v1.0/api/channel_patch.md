# <a name="patch-channel"></a><span data-ttu-id="3ae90-101">Patch-Kanal</span><span class="sxs-lookup"><span data-stu-id="3ae90-101">Patch channel</span></span>



<span data-ttu-id="3ae90-102">Aktualisieren Sie die Eigenschaften des angegebenen [DDE-Kanal](../resources/channel.md)an.</span><span class="sxs-lookup"><span data-stu-id="3ae90-102">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="3ae90-103">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="3ae90-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="3ae90-104">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="3ae90-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ae90-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3ae90-105">Permissions</span></span>
<span data-ttu-id="3ae90-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ae90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ae90-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ae90-108">Permission type</span></span>      | <span data-ttu-id="3ae90-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ae90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ae90-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ae90-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ae90-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae90-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ae90-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ae90-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ae90-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ae90-113">Not supported.</span></span>    |
|<span data-ttu-id="3ae90-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ae90-114">Application</span></span> | <span data-ttu-id="3ae90-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae90-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ae90-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ae90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3ae90-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ae90-117">Request headers</span></span>
| <span data-ttu-id="3ae90-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ae90-118">Header</span></span>       | <span data-ttu-id="3ae90-119">Wert</span><span class="sxs-lookup"><span data-stu-id="3ae90-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ae90-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ae90-120">Authorization</span></span>  | <span data-ttu-id="3ae90-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ae90-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ae90-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ae90-123">Content-Type</span></span>  | <span data-ttu-id="3ae90-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3ae90-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ae90-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ae90-125">Request body</span></span>
<span data-ttu-id="3ae90-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ae90-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ae90-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ae90-127">Response</span></span>

<span data-ttu-id="3ae90-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ae90-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ae90-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ae90-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ae90-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ae90-130">Request</span></span>
<span data-ttu-id="3ae90-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ae90-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="3ae90-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ae90-132">Response</span></span>
<span data-ttu-id="3ae90-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ae90-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
