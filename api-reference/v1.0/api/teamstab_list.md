# <a name="list-tabs-in-channel"></a><span data-ttu-id="a0010-101">Liste der Registerkarten im Kanal</span><span class="sxs-lookup"><span data-stu-id="a0010-101">List tabs in channel</span></span>



<span data-ttu-id="a0010-102">Rufen Sie die Liste der [Registerkarten](../resources/teamstab.md) in den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md)ab.</span><span class="sxs-lookup"><span data-stu-id="a0010-102">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a0010-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0010-103">Permissions</span></span>
<span data-ttu-id="a0010-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a0010-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0010-106">Permission type</span></span>      | <span data-ttu-id="a0010-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0010-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0010-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0010-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a0010-109">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0010-109">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="a0010-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0010-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0010-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0010-111">Not supported.</span></span>    |
| <span data-ttu-id="a0010-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0010-112">Application</span></span>                            | <span data-ttu-id="a0010-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0010-113">Group.Read.All, Group.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="a0010-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0010-114">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0010-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a0010-115">Optional query parameters</span></span>

<span data-ttu-id="a0010-116">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="a0010-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0010-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0010-117">Request headers</span></span>
| <span data-ttu-id="a0010-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0010-118">Header</span></span>       | <span data-ttu-id="a0010-119">Wert</span><span class="sxs-lookup"><span data-stu-id="a0010-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0010-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0010-120">Authorization</span></span>  | <span data-ttu-id="a0010-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0010-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0010-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0010-123">Request body</span></span>
<span data-ttu-id="a0010-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a0010-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0010-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0010-125">Response</span></span>
<span data-ttu-id="a0010-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Registerkarten](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="a0010-126">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0010-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0010-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0010-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0010-128">Request</span></span>
<span data-ttu-id="a0010-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0010-129">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="a0010-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0010-130">Response</span></span>
<span data-ttu-id="a0010-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0010-131">The following is an example of the response.</span></span>
><span data-ttu-id="a0010-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a0010-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
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
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
