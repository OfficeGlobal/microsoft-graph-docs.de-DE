# <a name="get-channel"></a><span data-ttu-id="1443c-101">Abrufen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="1443c-101">Get channel</span></span>



<span data-ttu-id="1443c-102">Abrufen der Eigenschaften und die Beziehungen eines [DDE-Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="1443c-102">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1443c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1443c-103">Permissions</span></span>
<span data-ttu-id="1443c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1443c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1443c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1443c-106">Permission type</span></span>      | <span data-ttu-id="1443c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1443c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1443c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1443c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1443c-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1443c-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1443c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1443c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1443c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1443c-111">Not supported.</span></span>    |
|<span data-ttu-id="1443c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1443c-112">Application</span></span> | <span data-ttu-id="1443c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1443c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="1443c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1443c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="1443c-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1443c-115">Optional query parameters</span></span>

<span data-ttu-id="1443c-116">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="1443c-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1443c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1443c-117">Request headers</span></span>
| <span data-ttu-id="1443c-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1443c-118">Header</span></span>       | <span data-ttu-id="1443c-119">Wert</span><span class="sxs-lookup"><span data-stu-id="1443c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1443c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1443c-120">Authorization</span></span>  | <span data-ttu-id="1443c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1443c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1443c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1443c-123">Request body</span></span>
<span data-ttu-id="1443c-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1443c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1443c-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="1443c-125">Response</span></span>

<span data-ttu-id="1443c-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Channel](../resources/channel.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1443c-126">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1443c-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1443c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1443c-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1443c-128">Request</span></span>
<span data-ttu-id="1443c-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1443c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="1443c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1443c-130">Response</span></span>
<span data-ttu-id="1443c-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1443c-131">Here is an example of the response.</span></span> 

><span data-ttu-id="1443c-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1443c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
