# <a name="list-groups"></a><span data-ttu-id="cf4af-101">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="cf4af-101">List groups</span></span>

<span data-ttu-id="cf4af-p101">Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen. Die [Standardeigenschaften](../api/group_get.md#default-properties) jeder einzelnen Gruppe werden zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf4af-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="cf4af-104">Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an:</span><span class="sxs-lookup"><span data-stu-id="cf4af-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="cf4af-105">Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="cf4af-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="permissions"></a><span data-ttu-id="cf4af-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf4af-106">Permissions</span></span>
<span data-ttu-id="cf4af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf4af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf4af-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf4af-109">Permission type</span></span>      | <span data-ttu-id="cf4af-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf4af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf4af-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf4af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf4af-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4af-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf4af-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf4af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf4af-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf4af-114">Not supported.</span></span>    |
|<span data-ttu-id="cf4af-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf4af-115">Application</span></span> | <span data-ttu-id="cf4af-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4af-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf4af-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf4af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf4af-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf4af-118">Optional query parameters</span></span>
<span data-ttu-id="cf4af-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf4af-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf4af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf4af-120">Request headers</span></span>
| <span data-ttu-id="cf4af-121">Name</span><span class="sxs-lookup"><span data-stu-id="cf4af-121">Name</span></span>       | <span data-ttu-id="cf4af-122">Typ</span><span class="sxs-lookup"><span data-stu-id="cf4af-122">Type</span></span> | <span data-ttu-id="cf4af-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf4af-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf4af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf4af-124">Authorization</span></span>  | <span data-ttu-id="cf4af-125">string</span><span class="sxs-lookup"><span data-stu-id="cf4af-125">string</span></span>  | <span data-ttu-id="cf4af-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf4af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf4af-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf4af-128">Request body</span></span>
<span data-ttu-id="cf4af-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf4af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf4af-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf4af-130">Response</span></span>

<span data-ttu-id="cf4af-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf4af-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf4af-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf4af-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf4af-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf4af-133">Request</span></span>
<span data-ttu-id="cf4af-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf4af-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a><span data-ttu-id="cf4af-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf4af-135">Response</span></span>
<span data-ttu-id="cf4af-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf4af-136">Here is an example of the response.</span></span>

<span data-ttu-id="cf4af-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden die [Standardeigenschaften](../api/group_get.md#default-properties) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf4af-p104">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
