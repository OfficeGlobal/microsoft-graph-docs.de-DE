# <a name="list-conversations"></a><span data-ttu-id="08d7e-101">Unterhaltungen auflisten</span><span class="sxs-lookup"><span data-stu-id="08d7e-101">List conversations</span></span>
<span data-ttu-id="08d7e-102">Mit dieser API können Sie eine Liste aller [Unterhaltungen](../resources/conversation.md) in einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="08d7e-102">Retrieve the list of conversations in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="08d7e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="08d7e-103">Permissions</span></span>
<span data-ttu-id="08d7e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="08d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="08d7e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08d7e-106">Permission type</span></span>      | <span data-ttu-id="08d7e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08d7e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08d7e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08d7e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="08d7e-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d7e-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08d7e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08d7e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08d7e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08d7e-111">Not supported.</span></span>    |
|<span data-ttu-id="08d7e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08d7e-112">Application</span></span> | <span data-ttu-id="08d7e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08d7e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08d7e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08d7e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08d7e-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="08d7e-115">Optional query parameters</span></span>
<span data-ttu-id="08d7e-116">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08d7e-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08d7e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08d7e-117">Request headers</span></span>
| <span data-ttu-id="08d7e-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="08d7e-118">Header</span></span>       | <span data-ttu-id="08d7e-119">Wert</span><span class="sxs-lookup"><span data-stu-id="08d7e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08d7e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="08d7e-120">Authorization</span></span>  | <span data-ttu-id="08d7e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08d7e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08d7e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08d7e-123">Request body</span></span>
<span data-ttu-id="08d7e-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="08d7e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08d7e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="08d7e-125">Response</span></span>
<span data-ttu-id="08d7e-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [conversation](../resources/conversation.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08d7e-126">If successful, this method returns a `200 OK` response code and collection of [Conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08d7e-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08d7e-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="08d7e-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08d7e-128">Request</span></span>
<span data-ttu-id="08d7e-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08d7e-129">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="08d7e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="08d7e-130">Response</span></span>
<span data-ttu-id="08d7e-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="08d7e-131">Here is an example of the response.</span></span>
><span data-ttu-id="08d7e-132">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="08d7e-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="08d7e-133">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="08d7e-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->