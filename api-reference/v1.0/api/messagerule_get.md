# <a name="get-rule"></a><span data-ttu-id="ce8c6-101">Regel abrufen</span><span class="sxs-lookup"><span data-stu-id="ce8c6-101">Get rule</span></span>


<span data-ttu-id="ce8c6-102">Abrufen der Eigenschaften und Beziehungen eines [messageRule](../resources/messagerule.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-102">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="ce8c6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce8c6-103">Permissions</span></span>
<span data-ttu-id="ce8c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce8c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce8c6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce8c6-106">Permission type</span></span>      | <span data-ttu-id="ce8c6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce8c6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce8c6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce8c6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ce8c6-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8c6-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ce8c6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce8c6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce8c6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8c6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ce8c6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce8c6-112">Application</span></span> | <span data-ttu-id="ce8c6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ce8c6-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce8c6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce8c6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce8c6-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ce8c6-115">Optional query parameters</span></span>
<span data-ttu-id="ce8c6-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce8c6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce8c6-117">Request headers</span></span>
| <span data-ttu-id="ce8c6-118">Name</span><span class="sxs-lookup"><span data-stu-id="ce8c6-118">Name</span></span>      |<span data-ttu-id="ce8c6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce8c6-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce8c6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce8c6-120">Authorization</span></span>  | <span data-ttu-id="ce8c6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ce8c6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce8c6-123">Request body</span></span>
<span data-ttu-id="ce8c6-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce8c6-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce8c6-125">Response</span></span>
<span data-ttu-id="ce8c6-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [messageRule](../resources/messagerule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-126">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce8c6-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce8c6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce8c6-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce8c6-128">Request</span></span>
<span data-ttu-id="ce8c6-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="ce8c6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce8c6-130">Response</span></span>
<span data-ttu-id="ce8c6-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-131">Here is an example of the response.</span></span> <span data-ttu-id="ce8c6-132">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-132">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="ce8c6-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce8c6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->