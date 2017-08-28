# <a name="send-mail"></a><span data-ttu-id="9041d-101">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="9041d-101">Send mail</span></span>

<span data-ttu-id="9041d-p101">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="9041d-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="9041d-104">Sie können in denselben Aktionsaufruf des Typs **sendMail** auch eine [Dateianlage](../resources/fileattachment.md) einschließen.</span><span class="sxs-lookup"><span data-stu-id="9041d-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="9041d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9041d-105">Permissions</span></span>
<span data-ttu-id="9041d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9041d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9041d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9041d-108">Permission type</span></span>      | <span data-ttu-id="9041d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9041d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9041d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9041d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9041d-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9041d-111">Mail.Send</span></span>    |
|<span data-ttu-id="9041d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9041d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9041d-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9041d-113">Mail.Send</span></span>    |
|<span data-ttu-id="9041d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9041d-114">Application</span></span> | <span data-ttu-id="9041d-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9041d-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9041d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9041d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="9041d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9041d-117">Request headers</span></span>
| <span data-ttu-id="9041d-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9041d-118">Header</span></span>       | <span data-ttu-id="9041d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9041d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9041d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9041d-120">Authorization</span></span>  | <span data-ttu-id="9041d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9041d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9041d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9041d-123">Content-Type</span></span>  | <span data-ttu-id="9041d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9041d-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9041d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9041d-125">Request body</span></span>
<span data-ttu-id="9041d-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9041d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9041d-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="9041d-127">Parameter</span></span>    | <span data-ttu-id="9041d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="9041d-128">Type</span></span>   |<span data-ttu-id="9041d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9041d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9041d-130">Nachricht</span><span class="sxs-lookup"><span data-stu-id="9041d-130">Message</span></span>|[<span data-ttu-id="9041d-131">message</span><span class="sxs-lookup"><span data-stu-id="9041d-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="9041d-p104">Die zu sendende Nachricht. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="9041d-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="9041d-134">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="9041d-134">SaveToSentItems</span></span>|<span data-ttu-id="9041d-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9041d-135">Boolean</span></span>|<span data-ttu-id="9041d-p105">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="9041d-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9041d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9041d-139">Response</span></span>

<span data-ttu-id="9041d-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9041d-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9041d-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9041d-142">Example</span></span>
<span data-ttu-id="9041d-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9041d-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9041d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9041d-144">Request</span></span>
<span data-ttu-id="9041d-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9041d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response"></a><span data-ttu-id="9041d-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="9041d-146">Response</span></span>
<span data-ttu-id="9041d-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9041d-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
