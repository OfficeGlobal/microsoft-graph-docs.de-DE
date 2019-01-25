---
title: Nachrichten senden
description: Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afa50b466bd7a90af4fedbdad4c5f7c5b4627b8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517211"
---
# <a name="send-mail"></a><span data-ttu-id="bc4a8-104">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="bc4a8-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc4a8-p102">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="bc4a8-107">In den gleichen Anruf **SendMail** -Aktion können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="bc4a8-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="bc4a8-108">Fügen Sie eine [Anlage](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a8-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="bc4a8-109">Rufen Sie einen anderen Benutzer in der neuen Nachricht mithilfe einer [erwähnen](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a8-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="bc4a8-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc4a8-110">Permissions</span></span>
<span data-ttu-id="bc4a8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc4a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bc4a8-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc4a8-113">Permission type</span></span>      | <span data-ttu-id="bc4a8-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc4a8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc4a8-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc4a8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bc4a8-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bc4a8-116">Mail.Send</span></span>    |
|<span data-ttu-id="bc4a8-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc4a8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc4a8-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bc4a8-118">Mail.Send</span></span>    |
|<span data-ttu-id="bc4a8-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc4a8-119">Application</span></span> | <span data-ttu-id="bc4a8-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="bc4a8-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc4a8-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc4a8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="bc4a8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc4a8-122">Request headers</span></span>
| <span data-ttu-id="bc4a8-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc4a8-123">Header</span></span>       | <span data-ttu-id="bc4a8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="bc4a8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc4a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc4a8-125">Authorization</span></span>  | <span data-ttu-id="bc4a8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc4a8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc4a8-128">Content-Type</span></span>  | <span data-ttu-id="bc4a8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bc4a8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc4a8-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc4a8-130">Request body</span></span>
<span data-ttu-id="bc4a8-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc4a8-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="bc4a8-132">Parameter</span></span>    | <span data-ttu-id="bc4a8-133">Typ</span><span class="sxs-lookup"><span data-stu-id="bc4a8-133">Type</span></span>   |<span data-ttu-id="bc4a8-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc4a8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc4a8-135">Nachricht</span><span class="sxs-lookup"><span data-stu-id="bc4a8-135">Message</span></span>|[<span data-ttu-id="bc4a8-136">message</span><span class="sxs-lookup"><span data-stu-id="bc4a8-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="bc4a8-p105">Die zu sendende Nachricht. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bc4a8-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="bc4a8-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="bc4a8-139">SaveToSentItems</span></span>|<span data-ttu-id="bc4a8-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc4a8-140">Boolean</span></span>|<span data-ttu-id="bc4a8-p106">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="bc4a8-144">Wenn Sie **erwähnen** aufrufen, um einen anderen Benutzer in der neuen Nachricht verwenden möchten:</span><span class="sxs-lookup"><span data-stu-id="bc4a8-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="bc4a8-145">Enthalten Sie die erforderlichen **ToRecipients** -Eigenschaft, die **erwähnungen** -Eigenschaft und alle schreibbaren Eigenschaften im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="bc4a8-146">Für jede erwähnt werden in der Eigenschaft **erwähnt** müssen Sie die **erwähnten** -Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="bc4a8-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc4a8-147">Response</span></span>

<span data-ttu-id="bc4a8-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc4a8-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc4a8-150">Example</span></span>
<span data-ttu-id="bc4a8-151">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="bc4a8-152">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="bc4a8-152">Request 1</span></span>
<span data-ttu-id="bc4a8-153">Es folgt ein Beispiel der Anforderung zum Erstellen und senden eine Nachricht im laufenden Betrieb.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="bc4a8-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="bc4a8-154">Response 1</span></span>
<span data-ttu-id="bc4a8-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="bc4a8-156">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="bc4a8-156">Request 2</span></span>
<span data-ttu-id="bc4a8-157">Das nächste Beispiel zeigt eine Meldung vom angemeldeten Benutzer auf Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-157">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="bc4a8-158">Die Nachricht enthält außerdem eine Erwähnung eines anderen Benutzers, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-158">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="bc4a8-159">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="bc4a8-159">Response 2</span></span>
<span data-ttu-id="bc4a8-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="bc4a8-161">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="bc4a8-161">Request 3</span></span>
<span data-ttu-id="bc4a8-162">Im nächsten Beispiel wird eine Meldung mit benutzerdefinierten Internetkopfzeilen Nachricht erstellt und sendet die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-162">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="bc4a8-163">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="bc4a8-163">Response 3</span></span>
<span data-ttu-id="bc4a8-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc4a8-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
