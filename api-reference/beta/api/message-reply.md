---
title: 'message: reply'
description: 'Antwort an den Absender einer Nachricht, einen Kommentar hinzufügen oder ändern aktualisierbaren Eigenschaften alle in eine **Antwort** Anruf. '
localization_priority: Normal
ms.openlocfilehash: 3844969c8c4bbec9026aee8477db968d5a3b0e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827461"
---
# <a name="message-reply"></a><span data-ttu-id="60ea1-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="60ea1-103">message: reply</span></span>

> <span data-ttu-id="60ea1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60ea1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60ea1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60ea1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60ea1-p102">Antwortet dem Absender einer Nachricht, fügt einen Kommentar hinzu oder ändert aktualisierbare Eigenschaften in einem **reply**-Aufruf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="60ea1-p102">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="60ea1-108">Alternativ können Sie zunächst [den Entwurf einer Antwortnachricht erstellen](../api/message-createreply.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Eigenschaften der Nachricht, und die Antwort zu [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="60ea1-108">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="60ea1-109">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="60ea1-109">**Note**</span></span>

- <span data-ttu-id="60ea1-110">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="60ea1-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="60ea1-111">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="60ea1-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="60ea1-112">Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie in **ReplyTo** und nicht der Empfänger in der Eigenschaft **aus** die Antwort an den Empfänger senden.</span><span class="sxs-lookup"><span data-stu-id="60ea1-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="60ea1-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60ea1-113">Permissions</span></span>
<span data-ttu-id="60ea1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60ea1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ea1-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60ea1-116">Permission type</span></span>      | <span data-ttu-id="60ea1-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60ea1-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ea1-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60ea1-118">Delegated (work or school account)</span></span> | <span data-ttu-id="60ea1-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60ea1-119">Mail.Send</span></span>    |
|<span data-ttu-id="60ea1-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60ea1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ea1-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60ea1-121">Mail.Send</span></span>    |
|<span data-ttu-id="60ea1-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60ea1-122">Application</span></span> | <span data-ttu-id="60ea1-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="60ea1-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ea1-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60ea1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="60ea1-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60ea1-125">Request headers</span></span>
| <span data-ttu-id="60ea1-126">Name</span><span class="sxs-lookup"><span data-stu-id="60ea1-126">Name</span></span>       | <span data-ttu-id="60ea1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="60ea1-127">Type</span></span> | <span data-ttu-id="60ea1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60ea1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60ea1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ea1-129">Authorization</span></span>  | <span data-ttu-id="60ea1-130">string</span><span class="sxs-lookup"><span data-stu-id="60ea1-130">string</span></span>  | <span data-ttu-id="60ea1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60ea1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60ea1-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60ea1-133">Content-Type</span></span> | <span data-ttu-id="60ea1-134">string</span><span class="sxs-lookup"><span data-stu-id="60ea1-134">string</span></span>  | <span data-ttu-id="60ea1-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60ea1-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ea1-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60ea1-137">Request body</span></span>
<span data-ttu-id="60ea1-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="60ea1-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60ea1-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="60ea1-139">Parameter</span></span>    | <span data-ttu-id="60ea1-140">Typ</span><span class="sxs-lookup"><span data-stu-id="60ea1-140">Type</span></span>   |<span data-ttu-id="60ea1-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60ea1-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60ea1-142">comment</span><span class="sxs-lookup"><span data-stu-id="60ea1-142">comment</span></span>|<span data-ttu-id="60ea1-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60ea1-143">String</span></span>|<span data-ttu-id="60ea1-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="60ea1-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="60ea1-146">message</span><span class="sxs-lookup"><span data-stu-id="60ea1-146">message</span></span>|[<span data-ttu-id="60ea1-147">message</span><span class="sxs-lookup"><span data-stu-id="60ea1-147">message</span></span>](../resources/message.md)|<span data-ttu-id="60ea1-148">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="60ea1-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="60ea1-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="60ea1-149">Response</span></span>

<span data-ttu-id="60ea1-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60ea1-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60ea1-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60ea1-152">Example</span></span>
<span data-ttu-id="60ea1-153">Das folgende Beispiel enthält einen Kommentar und Antwortnachricht einen Empfänger hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60ea1-153">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="60ea1-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60ea1-154">Request</span></span>
<span data-ttu-id="60ea1-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60ea1-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```

##### <a name="response"></a><span data-ttu-id="60ea1-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="60ea1-156">Response</span></span>
<span data-ttu-id="60ea1-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60ea1-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
