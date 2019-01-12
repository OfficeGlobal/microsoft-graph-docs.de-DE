---
title: Nachrichten senden
description: Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 48e6087cb8393bb4f679cabfe73d5cb280a71907
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991426"
---
# <a name="send-mail"></a><span data-ttu-id="8633e-104">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="8633e-104">Send mail</span></span>

> <span data-ttu-id="8633e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8633e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8633e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8633e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8633e-p103">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="8633e-p103">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="8633e-109">In den gleichen Anruf **SendMail** -Aktion können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="8633e-109">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="8633e-110">Fügen Sie eine [Anlage](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="8633e-110">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="8633e-111">Rufen Sie einen anderen Benutzer in der neuen Nachricht mithilfe einer [erwähnen](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="8633e-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="8633e-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8633e-112">Permissions</span></span>
<span data-ttu-id="8633e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8633e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8633e-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8633e-115">Permission type</span></span>      | <span data-ttu-id="8633e-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8633e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8633e-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8633e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8633e-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8633e-118">Mail.Send</span></span>    |
|<span data-ttu-id="8633e-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8633e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8633e-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8633e-120">Mail.Send</span></span>    |
|<span data-ttu-id="8633e-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8633e-121">Application</span></span> | <span data-ttu-id="8633e-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8633e-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8633e-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8633e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="8633e-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8633e-124">Request headers</span></span>
| <span data-ttu-id="8633e-125">Header</span><span class="sxs-lookup"><span data-stu-id="8633e-125">Header</span></span>       | <span data-ttu-id="8633e-126">Wert</span><span class="sxs-lookup"><span data-stu-id="8633e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8633e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8633e-127">Authorization</span></span>  | <span data-ttu-id="8633e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8633e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8633e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8633e-130">Content-Type</span></span>  | <span data-ttu-id="8633e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="8633e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8633e-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8633e-132">Request body</span></span>
<span data-ttu-id="8633e-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8633e-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8633e-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="8633e-134">Parameter</span></span>    | <span data-ttu-id="8633e-135">Typ</span><span class="sxs-lookup"><span data-stu-id="8633e-135">Type</span></span>   |<span data-ttu-id="8633e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8633e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8633e-137">Nachricht</span><span class="sxs-lookup"><span data-stu-id="8633e-137">Message</span></span>|[<span data-ttu-id="8633e-138">message</span><span class="sxs-lookup"><span data-stu-id="8633e-138">Message</span></span>](../resources/message.md)|<span data-ttu-id="8633e-p106">Die zu sendende Nachricht. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="8633e-p106">The message to send. Required.</span></span>|
|<span data-ttu-id="8633e-141">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="8633e-141">SaveToSentItems</span></span>|<span data-ttu-id="8633e-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8633e-142">Boolean</span></span>|<span data-ttu-id="8633e-p107">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="8633e-p107">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="8633e-146">Wenn Sie **erwähnen** aufrufen, um einen anderen Benutzer in der neuen Nachricht verwenden möchten:</span><span class="sxs-lookup"><span data-stu-id="8633e-146">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="8633e-147">Enthalten Sie die erforderlichen **ToRecipients** -Eigenschaft, die **erwähnungen** -Eigenschaft und alle schreibbaren Eigenschaften im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8633e-147">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="8633e-148">Für jede erwähnt werden in der Eigenschaft **erwähnt** müssen Sie die **erwähnten** -Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="8633e-148">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="8633e-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8633e-149">Response</span></span>

<span data-ttu-id="8633e-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8633e-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8633e-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8633e-152">Example</span></span>
<span data-ttu-id="8633e-153">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8633e-153">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="8633e-154">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="8633e-154">Request 1</span></span>
<span data-ttu-id="8633e-155">Es folgt ein Beispiel der Anforderung zum Erstellen und senden eine Nachricht im laufenden Betrieb.</span><span class="sxs-lookup"><span data-stu-id="8633e-155">Here is an example of the request to create and send a message on the fly.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
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
          "address": "samanthab@contoso.onmicrosoft.com"
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

##### <a name="response-1"></a><span data-ttu-id="8633e-156">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="8633e-156">Response 1</span></span>
<span data-ttu-id="8633e-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8633e-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="8633e-158">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="8633e-158">Request 2</span></span>
<span data-ttu-id="8633e-159">Das nächste Beispiel zeigt eine Meldung vom angemeldeten Benutzer auf Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="8633e-159">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="8633e-160">Die Nachricht enthält außerdem eine Erwähnung eines anderen Benutzers, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="8633e-160">The message also includes a mention of another user, Dana Swope.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="8633e-161">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="8633e-161">Response 2</span></span>
<span data-ttu-id="8633e-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8633e-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="8633e-163">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="8633e-163">Request 3</span></span>
<span data-ttu-id="8633e-164">Im nächsten Beispiel wird eine Meldung mit benutzerdefinierten Internetkopfzeilen Nachricht erstellt und sendet die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="8633e-164">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
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

##### <a name="response-3"></a><span data-ttu-id="8633e-165">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="8633e-165">Response 3</span></span>
<span data-ttu-id="8633e-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8633e-166">Here is an example of the response.</span></span>
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
