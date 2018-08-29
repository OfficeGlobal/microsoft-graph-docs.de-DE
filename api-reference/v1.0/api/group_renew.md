# <a name="group-renew"></a><span data-ttu-id="9a7db-101">group: renew</span><span class="sxs-lookup"><span data-stu-id="9a7db-101">group: renew</span></span>

<span data-ttu-id="9a7db-102">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="9a7db-102">Renews a group's expiration.</span></span> <span data-ttu-id="9a7db-103">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="9a7db-103">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a7db-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a7db-104">Permissions</span></span>

<span data-ttu-id="9a7db-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a7db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="9a7db-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a7db-107">Permission type</span></span>      | <span data-ttu-id="9a7db-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a7db-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a7db-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a7db-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9a7db-110">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a7db-110">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a7db-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a7db-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a7db-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a7db-112">Not supported</span></span> |
|<span data-ttu-id="9a7db-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a7db-113">Application</span></span> | <span data-ttu-id="9a7db-114">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a7db-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a7db-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a7db-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="9a7db-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a7db-116">Request headers</span></span>
| <span data-ttu-id="9a7db-117">Name</span><span class="sxs-lookup"><span data-stu-id="9a7db-117">Name</span></span>       | <span data-ttu-id="9a7db-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a7db-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a7db-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a7db-119">Authorization</span></span>  | <span data-ttu-id="9a7db-120">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9a7db-120">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="9a7db-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a7db-121">Request body</span></span>

<span data-ttu-id="9a7db-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a7db-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a7db-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a7db-123">Response</span></span>

<span data-ttu-id="9a7db-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a7db-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a7db-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a7db-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9a7db-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a7db-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="9a7db-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a7db-128">Response</span></span>
<span data-ttu-id="9a7db-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a7db-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->