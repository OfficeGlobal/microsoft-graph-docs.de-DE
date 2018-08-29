# <a name="get-conversation"></a><span data-ttu-id="6c3bd-101">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="6c3bd-101">Get conversation</span></span>
<span data-ttu-id="6c3bd-102">Abrufen eines [conversation](../resources/conversation.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-102">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c3bd-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6c3bd-103">Permissions</span></span>
<span data-ttu-id="6c3bd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c3bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c3bd-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c3bd-106">Permission type</span></span>      | <span data-ttu-id="6c3bd-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c3bd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c3bd-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c3bd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6c3bd-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3bd-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c3bd-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c3bd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c3bd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c3bd-111">Not supported.</span></span>    |
|<span data-ttu-id="6c3bd-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c3bd-112">Application</span></span> | <span data-ttu-id="6c3bd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c3bd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c3bd-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c3bd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c3bd-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6c3bd-115">Optional query parameters</span></span>
<span data-ttu-id="6c3bd-116">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c3bd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c3bd-117">Request headers</span></span>
| <span data-ttu-id="6c3bd-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c3bd-118">Header</span></span>       | <span data-ttu-id="6c3bd-119">Wert</span><span class="sxs-lookup"><span data-stu-id="6c3bd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c3bd-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6c3bd-120">Authorization</span></span>  | <span data-ttu-id="6c3bd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c3bd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c3bd-123">Request body</span></span>
<span data-ttu-id="6c3bd-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c3bd-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c3bd-125">Response</span></span>
<span data-ttu-id="6c3bd-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-126">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c3bd-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c3bd-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6c3bd-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c3bd-128">Request</span></span>
<span data-ttu-id="6c3bd-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="6c3bd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c3bd-130">Response</span></span>
<span data-ttu-id="6c3bd-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-131">The following is an example of the response.</span></span>
><span data-ttu-id="6c3bd-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6c3bd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
