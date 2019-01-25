---
title: 'message: reply'
description: 'Antwort an den Absender einer Nachricht, einen Kommentar hinzufügen oder ändern aktualisierbaren Eigenschaften alle in eine **Antwort** Anruf. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6461d9735459ff9cf956820b00bb61a4d42d1ec0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519010"
---
# <a name="message-reply"></a><span data-ttu-id="11f98-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="11f98-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f98-p101">Antwortet dem Absender einer Nachricht, fügt einen Kommentar hinzu oder ändert aktualisierbare Eigenschaften in einem **reply**-Aufruf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="11f98-p101">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call. The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="11f98-106">Alternativ können Sie zunächst [den Entwurf einer Antwortnachricht erstellen](../api/message-createreply.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Eigenschaften der Nachricht, und die Antwort zu [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="11f98-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="11f98-107">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="11f98-107">**Note**</span></span>

- <span data-ttu-id="11f98-108">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="11f98-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="11f98-109">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="11f98-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="11f98-110">Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie in **ReplyTo** und nicht der Empfänger in der Eigenschaft **aus** die Antwort an den Empfänger senden.</span><span class="sxs-lookup"><span data-stu-id="11f98-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="11f98-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11f98-111">Permissions</span></span>
<span data-ttu-id="11f98-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11f98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f98-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11f98-114">Permission type</span></span>      | <span data-ttu-id="11f98-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11f98-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f98-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11f98-116">Delegated (work or school account)</span></span> | <span data-ttu-id="11f98-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11f98-117">Mail.Send</span></span>    |
|<span data-ttu-id="11f98-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11f98-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f98-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11f98-119">Mail.Send</span></span>    |
|<span data-ttu-id="11f98-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11f98-120">Application</span></span> | <span data-ttu-id="11f98-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="11f98-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f98-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11f98-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="11f98-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11f98-123">Request headers</span></span>
| <span data-ttu-id="11f98-124">Name</span><span class="sxs-lookup"><span data-stu-id="11f98-124">Name</span></span>       | <span data-ttu-id="11f98-125">Typ</span><span class="sxs-lookup"><span data-stu-id="11f98-125">Type</span></span> | <span data-ttu-id="11f98-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11f98-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11f98-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="11f98-127">Authorization</span></span>  | <span data-ttu-id="11f98-128">string</span><span class="sxs-lookup"><span data-stu-id="11f98-128">string</span></span>  | <span data-ttu-id="11f98-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11f98-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11f98-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11f98-131">Content-Type</span></span> | <span data-ttu-id="11f98-132">string</span><span class="sxs-lookup"><span data-stu-id="11f98-132">string</span></span>  | <span data-ttu-id="11f98-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11f98-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11f98-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11f98-135">Request body</span></span>
<span data-ttu-id="11f98-136">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="11f98-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11f98-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="11f98-137">Parameter</span></span>    | <span data-ttu-id="11f98-138">Typ</span><span class="sxs-lookup"><span data-stu-id="11f98-138">Type</span></span>   |<span data-ttu-id="11f98-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11f98-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11f98-140">comment</span><span class="sxs-lookup"><span data-stu-id="11f98-140">comment</span></span>|<span data-ttu-id="11f98-141">String</span><span class="sxs-lookup"><span data-stu-id="11f98-141">String</span></span>|<span data-ttu-id="11f98-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="11f98-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="11f98-144">message</span><span class="sxs-lookup"><span data-stu-id="11f98-144">message</span></span>|[<span data-ttu-id="11f98-145">Nachricht</span><span class="sxs-lookup"><span data-stu-id="11f98-145">message</span></span>](../resources/message.md)|<span data-ttu-id="11f98-146">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="11f98-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="11f98-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="11f98-147">Response</span></span>

<span data-ttu-id="11f98-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11f98-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f98-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11f98-150">Example</span></span>
<span data-ttu-id="11f98-151">Das folgende Beispiel enthält einen Kommentar und Antwortnachricht einen Empfänger hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="11f98-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="11f98-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11f98-152">Request</span></span>
<span data-ttu-id="11f98-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11f98-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="11f98-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="11f98-154">Response</span></span>
<span data-ttu-id="11f98-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11f98-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
