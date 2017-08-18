# <a name="list-rejectedsenders"></a><span data-ttu-id="044dc-101">rejectedSenders auflisten</span><span class="sxs-lookup"><span data-stu-id="044dc-101">List rejectedSenders</span></span>

<span data-ttu-id="044dc-102">Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.</span><span class="sxs-lookup"><span data-stu-id="044dc-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="044dc-p101">Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im GET-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="044dc-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="044dc-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="044dc-105">Prerequisites</span></span>
<span data-ttu-id="044dc-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:  *Group.Read.All* oder *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="044dc-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="044dc-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="044dc-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="044dc-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="044dc-108">Optional query parameters</span></span>
<span data-ttu-id="044dc-109">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="044dc-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="044dc-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="044dc-110">Request headers</span></span>
| <span data-ttu-id="044dc-111">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="044dc-111">Header</span></span>       | <span data-ttu-id="044dc-112">Wert</span><span class="sxs-lookup"><span data-stu-id="044dc-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="044dc-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="044dc-113">Authorization</span></span>  | <span data-ttu-id="044dc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="044dc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="044dc-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="044dc-116">Request body</span></span>
<span data-ttu-id="044dc-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="044dc-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="044dc-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="044dc-118">Response</span></span>

<span data-ttu-id="044dc-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="044dc-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="044dc-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="044dc-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="044dc-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="044dc-121">Request</span></span>
<span data-ttu-id="044dc-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="044dc-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="044dc-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="044dc-123">Response</span></span>
<span data-ttu-id="044dc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="044dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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