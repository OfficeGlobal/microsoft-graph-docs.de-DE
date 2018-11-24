# <a name="update-team"></a><span data-ttu-id="bef14-101">Update-team</span><span class="sxs-lookup"><span data-stu-id="bef14-101">Update team</span></span>



<span data-ttu-id="bef14-102">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bef14-102">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bef14-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bef14-103">Permissions</span></span>
<span data-ttu-id="bef14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bef14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bef14-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bef14-106">Permission type</span></span>      | <span data-ttu-id="bef14-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bef14-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bef14-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bef14-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bef14-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef14-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bef14-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bef14-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bef14-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bef14-111">Not supported.</span></span>    |
|<span data-ttu-id="bef14-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bef14-112">Application</span></span> | <span data-ttu-id="bef14-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef14-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="bef14-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bef14-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bef14-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bef14-115">Request headers</span></span>
| <span data-ttu-id="bef14-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bef14-116">Header</span></span>       | <span data-ttu-id="bef14-117">Wert</span><span class="sxs-lookup"><span data-stu-id="bef14-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bef14-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="bef14-118">Authorization</span></span>  | <span data-ttu-id="bef14-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bef14-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bef14-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bef14-121">Content-Type</span></span>  | <span data-ttu-id="bef14-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bef14-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bef14-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bef14-123">Request body</span></span>
<span data-ttu-id="bef14-124">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bef14-124">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bef14-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="bef14-125">Response</span></span>

<span data-ttu-id="bef14-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bef14-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bef14-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bef14-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bef14-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bef14-128">Request</span></span>
<span data-ttu-id="bef14-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bef14-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="bef14-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bef14-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
