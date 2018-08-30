# <a name="message-move"></a><span data-ttu-id="576e0-101">Nachricht: verschieben</span><span class="sxs-lookup"><span data-stu-id="576e0-101">message: move</span></span>

<span data-ttu-id="576e0-102">Mit dieser API können Sie Nachrichten in Ordner verschieben.</span><span class="sxs-lookup"><span data-stu-id="576e0-102">Move a DriveItem to a new folder</span></span> <span data-ttu-id="576e0-103">Sie erstellt eine neue Kopie der Nachricht im Zielordner und entfernt die ursprüngliche Nachricht.</span><span class="sxs-lookup"><span data-stu-id="576e0-103">Move the message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="576e0-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="576e0-104">Permissions</span></span>

<span data-ttu-id="576e0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="576e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="576e0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="576e0-107">Permission type</span></span> | <span data-ttu-id="576e0-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="576e0-108">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="576e0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="576e0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="576e0-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="576e0-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="576e0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="576e0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="576e0-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="576e0-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="576e0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="576e0-113">Application</span></span> | <span data-ttu-id="576e0-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="576e0-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="576e0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="576e0-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="576e0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="576e0-116">Request headers</span></span>

| <span data-ttu-id="576e0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="576e0-117">Header</span></span> | <span data-ttu-id="576e0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="576e0-118">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="576e0-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="576e0-119">Authorization</span></span> | <span data-ttu-id="576e0-120">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="576e0-120"></span></span> <span data-ttu-id="576e0-121">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="576e0-121">Required.</span></span> |
| <span data-ttu-id="576e0-122">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="576e0-122">Content-Type</span></span> | <span data-ttu-id="576e0-123">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="576e0-123"></span></span> <span data-ttu-id="576e0-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="576e0-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="576e0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="576e0-125">Request body</span></span>

<span data-ttu-id="576e0-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="576e0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="576e0-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="576e0-127">Parameter</span></span>   | <span data-ttu-id="576e0-128">Typ</span><span class="sxs-lookup"><span data-stu-id="576e0-128">Type</span></span> |<span data-ttu-id="576e0-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="576e0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="576e0-130">destinationId</span><span class="sxs-lookup"><span data-stu-id="576e0-130">destinationId</span></span>|<span data-ttu-id="576e0-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="576e0-131">String</span></span>|<span data-ttu-id="576e0-132">Die Zielordner-ID oder ein bekannter Ordnername.</span><span class="sxs-lookup"><span data-stu-id="576e0-132">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="576e0-133">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="576e0-133">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="576e0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="576e0-134">Response</span></span>

<span data-ttu-id="576e0-135">Wenn das Verfahren erfolgreich verläuft, werden im Antworttext der Antwortcode `201 Created` und eine [mailFolder](../resources/message.md)-Ressource zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="576e0-135">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="576e0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="576e0-136">Example</span></span>

<span data-ttu-id="576e0-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="576e0-137">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="576e0-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="576e0-138">Request</span></span>

<span data-ttu-id="576e0-139">Die folgende Anforderung verschiebt die angegebene Nachricht in den Ordner Gelöschte Objekte, der anhand seines Namens einwandfrei identifiziert werden kann `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="576e0-139">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="576e0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="576e0-140">Response</span></span>

<span data-ttu-id="576e0-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="576e0-141">Here is an example of the response.</span></span>

> <span data-ttu-id="576e0-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="576e0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
