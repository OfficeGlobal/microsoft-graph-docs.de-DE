# <a name="send-mail"></a><span data-ttu-id="af4c8-101">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="af4c8-101">Send mail</span></span>

<span data-ttu-id="af4c8-p101">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="af4c8-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="af4c8-104">Sie können in denselben Aktionsaufruf des Typs **sendMail** auch eine [Dateianlage](../resources/fileattachment.md) einschließen.</span><span class="sxs-lookup"><span data-stu-id="af4c8-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="af4c8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="af4c8-105">Permissions</span></span>
<span data-ttu-id="af4c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af4c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="af4c8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af4c8-108">Permission type</span></span>      | <span data-ttu-id="af4c8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af4c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af4c8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af4c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af4c8-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="af4c8-111">Mail.Send</span></span>    |
|<span data-ttu-id="af4c8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af4c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af4c8-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="af4c8-113">Mail.Send</span></span>    |
|<span data-ttu-id="af4c8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af4c8-114">Application</span></span> | <span data-ttu-id="af4c8-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="af4c8-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="af4c8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af4c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="af4c8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af4c8-117">Request headers</span></span>
| <span data-ttu-id="af4c8-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="af4c8-118">Header</span></span>       | <span data-ttu-id="af4c8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="af4c8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af4c8-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="af4c8-120">Authorization</span></span>  | <span data-ttu-id="af4c8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="af4c8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af4c8-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="af4c8-123">Content-Type</span></span>  | <span data-ttu-id="af4c8-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="af4c8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af4c8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af4c8-125">Request body</span></span>
<span data-ttu-id="af4c8-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="af4c8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af4c8-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="af4c8-127">Parameter</span></span>    | <span data-ttu-id="af4c8-128">Typ</span><span class="sxs-lookup"><span data-stu-id="af4c8-128">Type</span></span>   |<span data-ttu-id="af4c8-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af4c8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af4c8-130">Nachricht</span><span class="sxs-lookup"><span data-stu-id="af4c8-130">message</span></span>|[<span data-ttu-id="af4c8-131">Meldung</span><span class="sxs-lookup"><span data-stu-id="af4c8-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="af4c8-p104">Die zu sendende Nachricht. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="af4c8-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="af4c8-134">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="af4c8-134">SaveToSentItems</span></span>|<span data-ttu-id="af4c8-135">Boolesch</span><span class="sxs-lookup"><span data-stu-id="af4c8-135">Boolean</span></span>|<span data-ttu-id="af4c8-p105">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="af4c8-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="af4c8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="af4c8-139">Response</span></span>

<span data-ttu-id="af4c8-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af4c8-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af4c8-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af4c8-142">Example</span></span>
<span data-ttu-id="af4c8-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="af4c8-143">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="af4c8-144">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="af4c8-144">Request 1</span></span>
<span data-ttu-id="af4c8-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af4c8-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

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

##### <a name="response-1"></a><span data-ttu-id="af4c8-146">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="af4c8-146">Response 1</span></span>
<span data-ttu-id="af4c8-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="af4c8-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="af4c8-148">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="af4c8-148">Request 2</span></span>
<span data-ttu-id="af4c8-149">Im nächsten Beispiel wird eine Meldung mit benutzerdefinierten Internet-Nachrichten-Headern erstellt und die Nachricht gesendet.</span><span class="sxs-lookup"><span data-stu-id="af4c8-149">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="af4c8-150">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="af4c8-150">Response 2</span></span>
<span data-ttu-id="af4c8-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="af4c8-151">Here is an example of the response.</span></span>
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
