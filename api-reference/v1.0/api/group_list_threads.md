# <a name="list-threads"></a><span data-ttu-id="42ffb-101">Threads auflisten</span><span class="sxs-lookup"><span data-stu-id="42ffb-101">List threads</span></span>

<span data-ttu-id="42ffb-102">Ruft alle Threads einer Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="42ffb-102">Get all the threads of a group.</span></span>

<span data-ttu-id="42ffb-103">Hinweis: Sie können auch [Alle Threads einer Unterhaltung abrufen](conversation_list_threads.md).</span><span class="sxs-lookup"><span data-stu-id="42ffb-103">Note: You can also [get all the threads of a conversation](conversation_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="42ffb-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42ffb-104">Permissions</span></span>
<span data-ttu-id="42ffb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="42ffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="42ffb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42ffb-107">Permission type</span></span>      | <span data-ttu-id="42ffb-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42ffb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42ffb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42ffb-109">Delegated (work or school account)</span></span> | <span data-ttu-id="42ffb-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ffb-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42ffb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42ffb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42ffb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42ffb-112">Not supported.</span></span>    |
|<span data-ttu-id="42ffb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42ffb-113">Application</span></span> | <span data-ttu-id="42ffb-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ffb-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42ffb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42ffb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42ffb-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="42ffb-116">Optional query parameters</span></span>
<span data-ttu-id="42ffb-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="42ffb-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="42ffb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42ffb-118">Request headers</span></span>
| <span data-ttu-id="42ffb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="42ffb-119">Header</span></span>       | <span data-ttu-id="42ffb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="42ffb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42ffb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42ffb-121">Authorization</span></span>  | <span data-ttu-id="42ffb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42ffb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42ffb-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42ffb-124">Request body</span></span>
<span data-ttu-id="42ffb-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="42ffb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42ffb-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="42ffb-126">Response</span></span>

<span data-ttu-id="42ffb-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversationThread](../resources/conversationthread.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42ffb-127">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42ffb-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42ffb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42ffb-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42ffb-129">Request</span></span>
<span data-ttu-id="42ffb-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42ffb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="42ffb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="42ffb-131">Response</span></span>
<span data-ttu-id="42ffb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42ffb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
