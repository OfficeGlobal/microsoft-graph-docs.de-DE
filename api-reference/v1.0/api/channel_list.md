# <a name="list-channels"></a><span data-ttu-id="7eaec-101">Liste Kanäle</span><span class="sxs-lookup"><span data-stu-id="7eaec-101">List channels</span></span>



<span data-ttu-id="7eaec-102">Abrufen der Liste der [Kanäle](../resources/channel.md) in dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="7eaec-102">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="7eaec-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7eaec-103">Permissions</span></span>
<span data-ttu-id="7eaec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7eaec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7eaec-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7eaec-106">Permission type</span></span>      | <span data-ttu-id="7eaec-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7eaec-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eaec-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7eaec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7eaec-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eaec-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7eaec-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7eaec-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eaec-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7eaec-111">Not supported.</span></span>    |
|<span data-ttu-id="7eaec-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7eaec-112">Application</span></span> | <span data-ttu-id="7eaec-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eaec-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7eaec-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7eaec-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7eaec-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7eaec-115">Optional query parameters</span></span>
<span data-ttu-id="7eaec-116">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="7eaec-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7eaec-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7eaec-117">Request headers</span></span>
| <span data-ttu-id="7eaec-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7eaec-118">Header</span></span>       | <span data-ttu-id="7eaec-119">Wert</span><span class="sxs-lookup"><span data-stu-id="7eaec-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7eaec-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eaec-120">Authorization</span></span>  | <span data-ttu-id="7eaec-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7eaec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7eaec-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7eaec-123">Request body</span></span>
<span data-ttu-id="7eaec-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7eaec-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eaec-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="7eaec-125">Response</span></span>

<span data-ttu-id="7eaec-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DDE-Kanal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="7eaec-126">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eaec-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7eaec-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7eaec-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7eaec-128">Request</span></span>
<span data-ttu-id="7eaec-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7eaec-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="7eaec-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7eaec-130">Response</span></span>
<span data-ttu-id="7eaec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7eaec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
