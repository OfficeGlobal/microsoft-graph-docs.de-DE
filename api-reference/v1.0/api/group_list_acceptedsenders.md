# <a name="list-acceptedsenders"></a><span data-ttu-id="3a84a-101">acceptedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="3a84a-101">List acceptedSenders</span></span>

<span data-ttu-id="3a84a-102">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der acceptedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="3a84a-102">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="3a84a-p101">Benutzer in der Liste der zulässigenAbsender können Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3a84a-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a84a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a84a-105">Permissions</span></span>
<span data-ttu-id="3a84a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a84a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a84a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a84a-108">Permission type</span></span>      | <span data-ttu-id="3a84a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a84a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a84a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a84a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a84a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a84a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a84a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a84a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a84a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a84a-113">Not supported.</span></span>    |
|<span data-ttu-id="3a84a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a84a-114">Application</span></span> | <span data-ttu-id="3a84a-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a84a-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a84a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a84a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a84a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3a84a-117">Optional query parameters</span></span>
<span data-ttu-id="3a84a-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a84a-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3a84a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a84a-119">Request headers</span></span>
| <span data-ttu-id="3a84a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3a84a-120">Header</span></span>       | <span data-ttu-id="3a84a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3a84a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a84a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a84a-122">Authorization</span></span>  | <span data-ttu-id="3a84a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a84a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a84a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a84a-125">Request body</span></span>
<span data-ttu-id="3a84a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a84a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a84a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a84a-127">Response</span></span>

<span data-ttu-id="3a84a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a84a-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a84a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a84a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a84a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a84a-130">Request</span></span>
<span data-ttu-id="3a84a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a84a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```
##### <a name="response"></a><span data-ttu-id="3a84a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a84a-132">Response</span></span>
<span data-ttu-id="3a84a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a84a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->