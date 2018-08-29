# <a name="list-rules"></a><span data-ttu-id="d6dfe-101">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="d6dfe-101">List rules</span></span>

<span data-ttu-id="d6dfe-102">Ruft alle [messageRule](../resources/messagerule.md)-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-102">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6dfe-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d6dfe-103">Permissions</span></span>
<span data-ttu-id="d6dfe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6dfe-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6dfe-106">Permission type</span></span>      | <span data-ttu-id="d6dfe-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6dfe-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6dfe-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6dfe-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d6dfe-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d6dfe-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d6dfe-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6dfe-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6dfe-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d6dfe-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d6dfe-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6dfe-112">Application</span></span> | <span data-ttu-id="d6dfe-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d6dfe-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6dfe-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6dfe-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6dfe-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d6dfe-115">Optional query parameters</span></span>
<span data-ttu-id="d6dfe-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d6dfe-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6dfe-117">Request headers</span></span>
| <span data-ttu-id="d6dfe-118">Name</span><span class="sxs-lookup"><span data-stu-id="d6dfe-118">Name</span></span>       | <span data-ttu-id="d6dfe-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d6dfe-119">Type</span></span> | <span data-ttu-id="d6dfe-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6dfe-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6dfe-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d6dfe-121">Authorization</span></span>  | <span data-ttu-id="d6dfe-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6dfe-122">string</span></span>  | <span data-ttu-id="d6dfe-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6dfe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6dfe-125">Request body</span></span>
<span data-ttu-id="d6dfe-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d6dfe-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6dfe-127">Response</span></span>
<span data-ttu-id="d6dfe-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [messageRule](../resources/messagerule.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-128">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6dfe-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6dfe-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6dfe-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6dfe-130">Request</span></span>
<span data-ttu-id="d6dfe-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
##### <a name="response"></a><span data-ttu-id="d6dfe-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6dfe-132">Response</span></span>
<span data-ttu-id="d6dfe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6dfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
