# <a name="get-team"></a><span data-ttu-id="8ebb7-101">Get-team</span><span class="sxs-lookup"><span data-stu-id="8ebb7-101">Get team</span></span>



<span data-ttu-id="8ebb7-102">Abrufen der Eigenschaften und Beziehungen des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8ebb7-102">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ebb7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ebb7-103">Permissions</span></span>
<span data-ttu-id="8ebb7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ebb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ebb7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ebb7-106">Permission type</span></span>      | <span data-ttu-id="8ebb7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ebb7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ebb7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ebb7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8ebb7-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ebb7-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ebb7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ebb7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ebb7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ebb7-111">Not supported.</span></span>    |
|<span data-ttu-id="8ebb7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ebb7-112">Application</span></span> | <span data-ttu-id="8ebb7-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ebb7-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="8ebb7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ebb7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ebb7-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8ebb7-115">Optional query parameters</span></span>
<span data-ttu-id="8ebb7-116">Diese Methode unterstützt die $select und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-116">This method supports the $select and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ebb7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ebb7-117">Request headers</span></span>
| <span data-ttu-id="8ebb7-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8ebb7-118">Header</span></span>       | <span data-ttu-id="8ebb7-119">Wert</span><span class="sxs-lookup"><span data-stu-id="8ebb7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ebb7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ebb7-120">Authorization</span></span>  | <span data-ttu-id="8ebb7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ebb7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ebb7-123">Request body</span></span>
<span data-ttu-id="8ebb7-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ebb7-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ebb7-125">Response</span></span>

<span data-ttu-id="8ebb7-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-126">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ebb7-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ebb7-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8ebb7-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ebb7-128">Request</span></span>
<span data-ttu-id="8ebb7-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="8ebb7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ebb7-130">Response</span></span>
<span data-ttu-id="8ebb7-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-131">The following is an example of the response.</span></span> 

><span data-ttu-id="8ebb7-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8ebb7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
