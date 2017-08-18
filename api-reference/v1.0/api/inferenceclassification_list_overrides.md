# <a name="list-overrides"></a><span data-ttu-id="da13a-101">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="da13a-101">List overrides</span></span>

<span data-ttu-id="da13a-102">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="da13a-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="da13a-p101">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="da13a-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da13a-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="da13a-105">Prerequisites</span></span>
<span data-ttu-id="da13a-106">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="da13a-106">The following **scopes** are required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="da13a-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da13a-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="da13a-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da13a-108">Request headers</span></span>
| <span data-ttu-id="da13a-109">Name</span><span class="sxs-lookup"><span data-stu-id="da13a-109">Name</span></span>       | <span data-ttu-id="da13a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="da13a-110">Type</span></span> | <span data-ttu-id="da13a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da13a-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da13a-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="da13a-112">Authorization</span></span>  | <span data-ttu-id="da13a-113">string</span><span class="sxs-lookup"><span data-stu-id="da13a-113">string</span></span>  | <span data-ttu-id="da13a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da13a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da13a-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da13a-116">Request body</span></span>
<span data-ttu-id="da13a-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da13a-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da13a-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="da13a-118">Response</span></span>

<span data-ttu-id="da13a-p103">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekten im Antworttext zurückgegeben. Wenn der Benutzer keine Außerkraftsetzungen eingerichtet hat, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da13a-p103">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="da13a-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da13a-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da13a-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da13a-122">Request</span></span>
<span data-ttu-id="da13a-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da13a-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="da13a-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="da13a-124">Response</span></span>
<span data-ttu-id="da13a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da13a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Fanny Downs",
        "address": "fannyd@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->