# <a name="list-overrides"></a><span data-ttu-id="3923a-101">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="3923a-101">List overrides</span></span>

<span data-ttu-id="3923a-102">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="3923a-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="3923a-p101">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="3923a-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="3923a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3923a-105">Permissions</span></span>
<span data-ttu-id="3923a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3923a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3923a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3923a-108">Permission type</span></span>      | <span data-ttu-id="3923a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3923a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3923a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3923a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3923a-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3923a-111">Mail.Read</span></span>    |
|<span data-ttu-id="3923a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3923a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3923a-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3923a-113">Mail.Read</span></span>    |
|<span data-ttu-id="3923a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3923a-114">Application</span></span> | <span data-ttu-id="3923a-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3923a-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3923a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3923a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="3923a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3923a-117">Request headers</span></span>
| <span data-ttu-id="3923a-118">Name</span><span class="sxs-lookup"><span data-stu-id="3923a-118">Name</span></span>       | <span data-ttu-id="3923a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="3923a-119">Type</span></span> | <span data-ttu-id="3923a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3923a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3923a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3923a-121">Authorization</span></span>  | <span data-ttu-id="3923a-122">string</span><span class="sxs-lookup"><span data-stu-id="3923a-122">string</span></span>  | <span data-ttu-id="3923a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3923a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3923a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3923a-125">Request body</span></span>
<span data-ttu-id="3923a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3923a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3923a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3923a-127">Response</span></span>

<span data-ttu-id="3923a-p104">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekten im Antworttext zurückgegeben. Wenn der Benutzer keine Außerkraftsetzungen eingerichtet hat, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3923a-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="3923a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3923a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3923a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3923a-131">Request</span></span>
<span data-ttu-id="3923a-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3923a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="3923a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3923a-133">Response</span></span>
<span data-ttu-id="3923a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3923a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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