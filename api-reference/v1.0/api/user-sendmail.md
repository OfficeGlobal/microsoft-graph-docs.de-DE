---
title: Nachrichten senden
description: Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.
author: dkershaw10
ms.openlocfilehash: a818ec5cc455b6ca78c920be57ad34155a03a1bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333292"
---
# <a name="send-mail"></a><span data-ttu-id="48634-104">Nachrichten senden</span><span class="sxs-lookup"><span data-stu-id="48634-104">Send mail</span></span>

<span data-ttu-id="48634-p102">Sendet die im Anforderungstext angegebene Nachricht. Die Nachricht wird dann automatisch im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="48634-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="48634-107">Sie können in denselben Aktionsaufruf des Typs **sendMail** auch eine [Dateianlage](../resources/fileattachment.md) einschließen.</span><span class="sxs-lookup"><span data-stu-id="48634-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="48634-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48634-108">Permissions</span></span>
<span data-ttu-id="48634-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48634-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48634-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48634-111">Permission type</span></span>      | <span data-ttu-id="48634-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48634-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48634-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48634-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48634-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48634-114">Mail.Send</span></span>    |
|<span data-ttu-id="48634-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48634-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48634-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48634-116">Mail.Send</span></span>    |
|<span data-ttu-id="48634-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48634-117">Application</span></span> | <span data-ttu-id="48634-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48634-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="48634-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48634-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="48634-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48634-120">Request headers</span></span>
| <span data-ttu-id="48634-121">Header</span><span class="sxs-lookup"><span data-stu-id="48634-121">Header</span></span>       | <span data-ttu-id="48634-122">Wert</span><span class="sxs-lookup"><span data-stu-id="48634-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48634-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48634-123">Authorization</span></span>  | <span data-ttu-id="48634-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48634-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48634-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48634-126">Content-Type</span></span>  | <span data-ttu-id="48634-127">application/json</span><span class="sxs-lookup"><span data-stu-id="48634-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48634-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48634-128">Request body</span></span>
<span data-ttu-id="48634-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="48634-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48634-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="48634-130">Parameter</span></span>    | <span data-ttu-id="48634-131">Typ</span><span class="sxs-lookup"><span data-stu-id="48634-131">Type</span></span>   |<span data-ttu-id="48634-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48634-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48634-133">message</span><span class="sxs-lookup"><span data-stu-id="48634-133">message</span></span>|[<span data-ttu-id="48634-134">message</span><span class="sxs-lookup"><span data-stu-id="48634-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="48634-p105">Die zu sendende Nachricht. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="48634-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="48634-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="48634-137">saveToSentItems</span></span>|<span data-ttu-id="48634-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48634-138">Boolean</span></span>|<span data-ttu-id="48634-p106">,Gibt an, ob die Nachricht im Ordner „Gesendete Elemente“ gespeichert werden soll. Geben Sie es nur an, wenn der Parameter false ist; der Standardwert true ist.  Optional.</span><span class="sxs-lookup"><span data-stu-id="48634-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48634-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="48634-142">Response</span></span>

<span data-ttu-id="48634-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48634-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48634-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48634-145">Example</span></span>
<span data-ttu-id="48634-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="48634-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="48634-147">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="48634-147">Request 1</span></span>
<span data-ttu-id="48634-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48634-148">Here is an example of the request.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="48634-149">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="48634-149">Response 1</span></span>
<span data-ttu-id="48634-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48634-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="48634-151">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="48634-151">Request 2</span></span>
<span data-ttu-id="48634-152">Im nächsten Beispiel wird eine Meldung mit benutzerdefinierten Internetkopfzeilen Nachricht erstellt und sendet die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="48634-152">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="48634-153">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="48634-153">Response 2</span></span>
<span data-ttu-id="48634-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48634-154">Here is an example of the response.</span></span>
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
