# <a name="list-rejectedsenders"></a><span data-ttu-id="60e51-101">rejectedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="60e51-101">List rejectedSenders</span></span>
<span data-ttu-id="60e51-102">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="60e51-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="60e51-p101">Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="60e51-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="60e51-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60e51-105">Permissions</span></span>
<span data-ttu-id="60e51-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="60e51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60e51-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60e51-108">Permission type</span></span>      | <span data-ttu-id="60e51-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60e51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e51-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60e51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60e51-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e51-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60e51-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60e51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60e51-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60e51-113">Not supported.</span></span>    |
|<span data-ttu-id="60e51-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60e51-114">Application</span></span> | <span data-ttu-id="60e51-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60e51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60e51-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60e51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60e51-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="60e51-117">Optional query parameters</span></span>
<span data-ttu-id="60e51-118">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60e51-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60e51-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60e51-119">Request headers</span></span>
| <span data-ttu-id="60e51-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="60e51-120">Header</span></span>       | <span data-ttu-id="60e51-121">Wert</span><span class="sxs-lookup"><span data-stu-id="60e51-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60e51-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60e51-122">Authorization</span></span>  | <span data-ttu-id="60e51-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60e51-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60e51-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60e51-125">Request body</span></span>
<span data-ttu-id="60e51-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="60e51-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e51-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="60e51-127">Response</span></span>
<span data-ttu-id="60e51-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60e51-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e51-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60e51-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="60e51-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60e51-130">Request</span></span>
<span data-ttu-id="60e51-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60e51-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="60e51-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="60e51-132">Response</span></span>
<span data-ttu-id="60e51-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60e51-133">The following is an example of the response.</span></span>
><span data-ttu-id="60e51-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="60e51-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60e51-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="60e51-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->