# <a name="create-channel"></a><span data-ttu-id="b1c22-101">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="b1c22-101">Create Channel</span></span>



<span data-ttu-id="b1c22-102">Erstellen Sie einen neuen [Channel](../resources/channel.md) in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="b1c22-102">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="b1c22-103">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="b1c22-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="b1c22-104">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="b1c22-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c22-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1c22-105">Permissions</span></span>
<span data-ttu-id="b1c22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1c22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b1c22-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1c22-108">Permission type</span></span>      | <span data-ttu-id="b1c22-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1c22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1c22-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1c22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1c22-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c22-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1c22-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1c22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c22-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1c22-113">Not supported.</span></span>    |
|<span data-ttu-id="b1c22-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1c22-114">Application</span></span> | <span data-ttu-id="b1c22-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c22-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="b1c22-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1c22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="b1c22-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1c22-117">Request headers</span></span>
| <span data-ttu-id="b1c22-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1c22-118">Header</span></span>       | <span data-ttu-id="b1c22-119">Wert</span><span class="sxs-lookup"><span data-stu-id="b1c22-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1c22-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1c22-120">Authorization</span></span>  | <span data-ttu-id="b1c22-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1c22-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1c22-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1c22-123">Content-Type</span></span>  | <span data-ttu-id="b1c22-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c22-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1c22-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1c22-125">Request body</span></span>
<span data-ttu-id="b1c22-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1c22-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1c22-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1c22-127">Response</span></span>

<span data-ttu-id="b1c22-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Channel](../resources/channel.md) -Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b1c22-128">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1c22-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1c22-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1c22-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1c22-130">Request</span></span>
<span data-ttu-id="b1c22-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1c22-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="b1c22-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1c22-132">Response</span></span>
<span data-ttu-id="b1c22-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1c22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
