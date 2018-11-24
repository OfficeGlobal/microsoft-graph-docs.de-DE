# <a name="get-tab"></a><span data-ttu-id="a9f82-101">Erste Registerkarte</span><span class="sxs-lookup"><span data-stu-id="a9f82-101">Get tab</span></span>



<span data-ttu-id="a9f82-102">Abrufen der Eigenschaften und Beziehungen zwischen der angegebenen [Registerkarte](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="a9f82-102">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a9f82-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a9f82-103">Permissions</span></span>
<span data-ttu-id="a9f82-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9f82-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9f82-106">Permission type</span></span>      | <span data-ttu-id="a9f82-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9f82-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9f82-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9f82-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a9f82-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f82-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9f82-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9f82-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9f82-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9f82-111">Not supported.</span></span>    |
|<span data-ttu-id="a9f82-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9f82-112">Application</span></span> | <span data-ttu-id="a9f82-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f82-113">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="a9f82-114">Nur die [Berechtigungen delegiert](../../../concepts/permissions_reference.md) werden gegenwärtig unterstützt für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="a9f82-114">Currently, only [delegated permissions](../../../concepts/permissions_reference.md) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9f82-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9f82-115">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9f82-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a9f82-116">Optional query parameters</span></span>

<span data-ttu-id="a9f82-117">Diese Methode unterstützt die $select und $den [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="a9f82-117">This method supports the $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9f82-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9f82-118">Request headers</span></span>
| <span data-ttu-id="a9f82-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9f82-119">Header</span></span>       | <span data-ttu-id="a9f82-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a9f82-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9f82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f82-121">Authorization</span></span>  | <span data-ttu-id="a9f82-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a9f82-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9f82-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9f82-124">Request body</span></span>
<span data-ttu-id="a9f82-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9f82-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9f82-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9f82-126">Response</span></span>

<span data-ttu-id="a9f82-127">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Tab](../resources/teamstab.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a9f82-127">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9f82-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9f82-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a9f82-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9f82-129">Request</span></span>
<span data-ttu-id="a9f82-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9f82-130">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="a9f82-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9f82-131">Response</span></span>
<span data-ttu-id="a9f82-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a9f82-132">The following is an example of the response.</span></span> 

><span data-ttu-id="a9f82-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a9f82-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
