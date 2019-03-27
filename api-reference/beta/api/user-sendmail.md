---
title: Nachrichten senden
description: Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 47cdb200f7de493c6fcc83b3d77be2af1824ef65
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869428"
---
# <a name="send-mail"></a><span data-ttu-id="037f3-104">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="037f3-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="037f3-p102">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="037f3-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="037f3-107">Im gleichen **sendmail** -Aktionsaufruf haben Sie folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="037f3-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="037f3-108">Hinzufügen einer [Anlage](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="037f3-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="037f3-109">Verwenden einer [Erwähnung](../resources/mention.md) zum Aufrufen eines anderen Benutzers in der neuen Nachricht</span><span class="sxs-lookup"><span data-stu-id="037f3-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="037f3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="037f3-110">Permissions</span></span>
<span data-ttu-id="037f3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="037f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="037f3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="037f3-113">Permission type</span></span>      | <span data-ttu-id="037f3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="037f3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="037f3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="037f3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="037f3-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="037f3-116">Mail.Send</span></span>    |
|<span data-ttu-id="037f3-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="037f3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="037f3-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="037f3-118">Mail.Send</span></span>    |
|<span data-ttu-id="037f3-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="037f3-119">Application</span></span> | <span data-ttu-id="037f3-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="037f3-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="037f3-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="037f3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="037f3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="037f3-122">Request headers</span></span>
| <span data-ttu-id="037f3-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="037f3-123">Header</span></span>       | <span data-ttu-id="037f3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="037f3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="037f3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="037f3-125">Authorization</span></span>  | <span data-ttu-id="037f3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="037f3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="037f3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="037f3-128">Content-Type</span></span>  | <span data-ttu-id="037f3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="037f3-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="037f3-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="037f3-130">Request body</span></span>
<span data-ttu-id="037f3-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="037f3-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="037f3-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="037f3-132">Parameter</span></span>    | <span data-ttu-id="037f3-133">Typ</span><span class="sxs-lookup"><span data-stu-id="037f3-133">Type</span></span>   |<span data-ttu-id="037f3-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="037f3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="037f3-135">Nachricht</span><span class="sxs-lookup"><span data-stu-id="037f3-135">Message</span></span>|[<span data-ttu-id="037f3-136">message</span><span class="sxs-lookup"><span data-stu-id="037f3-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="037f3-p105">Die zu sendende Nachricht. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="037f3-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="037f3-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="037f3-139">SaveToSentItems</span></span>|<span data-ttu-id="037f3-140">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="037f3-140">Boolean</span></span>|<span data-ttu-id="037f3-p106">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="037f3-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="037f3-144">Wenn Sie **erwähnen** möchten, um einen anderen Benutzer in der neuen Nachricht aufzurufen:</span><span class="sxs-lookup"><span data-stu-id="037f3-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="037f3-145">Schließen Sie die \*\*\*\* erforderliche torecipients-Eigenschaft, die **Mentions** -Eigenschaft und alle beschreibbaren Nachrichteneigenschaften im Anforderungstext ein.</span><span class="sxs-lookup"><span data-stu-id="037f3-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="037f3-146">Für jede Erwähnung in \*\*\*\* der Mentions-Eigenschaft müssen Sie die **genannte** Eigenschaft angeben.</span><span class="sxs-lookup"><span data-stu-id="037f3-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="037f3-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="037f3-147">Response</span></span>

<span data-ttu-id="037f3-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="037f3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="037f3-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="037f3-150">Example</span></span>
<span data-ttu-id="037f3-151">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="037f3-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="037f3-152">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="037f3-152">Request 1</span></span>
<span data-ttu-id="037f3-153">Hier ist ein Beispiel für die Anforderung zum Erstellen und Senden einer Nachricht im Handumdrehen.</span><span class="sxs-lookup"><span data-stu-id="037f3-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="037f3-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="037f3-154">Response 1</span></span>
<span data-ttu-id="037f3-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="037f3-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="037f3-156">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="037f3-156">Request 2</span></span>
<span data-ttu-id="037f3-157">Im nächsten Beispiel wird eine Meldung des angemeldeten Benutzers an Samantha Booth angezeigt.</span><span class="sxs-lookup"><span data-stu-id="037f3-157">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="037f3-158">Die Nachricht enthält auch eine Erwähnung eines anderen Benutzers, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="037f3-158">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="037f3-159">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="037f3-159">Response 2</span></span>
<span data-ttu-id="037f3-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="037f3-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="037f3-161">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="037f3-161">Request 3</span></span>
<span data-ttu-id="037f3-162">Im nächsten Beispiel wird eine Nachricht mit benutzerdefinierten Internet Nachrichtenkopfzeilen erstellt und die Nachricht gesendet.</span><span class="sxs-lookup"><span data-stu-id="037f3-162">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="037f3-163">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="037f3-163">Response 3</span></span>
<span data-ttu-id="037f3-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="037f3-164">Here is an example of the response.</span></span>
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
