---
title: 'message: replyAll'
description: 'Antworten Sie an alle Empfänger einer Nachricht durch einen Kommentar angeben und keine aktualisierbaren Eigenschaften ändern '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1abbf271350c6bbbd10af1f17c6c7d3069c3cf22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976366"
---
# <a name="message-replyall"></a><span data-ttu-id="311b1-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="311b1-103">message: replyAll</span></span>

> <span data-ttu-id="311b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="311b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="311b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="311b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="311b1-106">Antworten Sie an alle Empfänger einer Nachricht durch einen Kommentar angeben und ändern keine aktualisierbaren Eigenschaften für die Antwort, die alle mithilfe der **ReplyAll** -Methode.</span><span class="sxs-lookup"><span data-stu-id="311b1-106">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="311b1-107">Die Nachricht wird im Ordner "Gesendete Elemente" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="311b1-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="311b1-108">Alternativ können Sie zunächst [Erstellen Sie eine Entwurf allen Antworten - Nachricht](../api/message-createreplyall.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Eigenschaften der Nachricht, und die Antwort zu [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="311b1-108">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="311b1-109">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="311b1-109">**Note**</span></span>

- <span data-ttu-id="311b1-110">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="311b1-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="311b1-111">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="311b1-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="311b1-112">Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie senden Sie die Antwort an die Empfänger in der</span><span class="sxs-lookup"><span data-stu-id="311b1-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="311b1-113">**ReplyTo** und **ToRecipients** -Eigenschaften, und nicht die Empfänger in den Eigenschaften **von** und **ToRecipients** .</span><span class="sxs-lookup"><span data-stu-id="311b1-113">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="311b1-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="311b1-114">Permissions</span></span>
<span data-ttu-id="311b1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="311b1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="311b1-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="311b1-117">Permission type</span></span>      | <span data-ttu-id="311b1-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="311b1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="311b1-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="311b1-119">Delegated (work or school account)</span></span> | <span data-ttu-id="311b1-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="311b1-120">Mail.Send</span></span>    |
|<span data-ttu-id="311b1-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="311b1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="311b1-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="311b1-122">Mail.Send</span></span>    |
|<span data-ttu-id="311b1-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="311b1-123">Application</span></span> | <span data-ttu-id="311b1-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="311b1-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="311b1-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="311b1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="311b1-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="311b1-126">Request headers</span></span>
| <span data-ttu-id="311b1-127">Name</span><span class="sxs-lookup"><span data-stu-id="311b1-127">Name</span></span>       | <span data-ttu-id="311b1-128">Typ</span><span class="sxs-lookup"><span data-stu-id="311b1-128">Type</span></span> | <span data-ttu-id="311b1-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="311b1-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="311b1-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="311b1-130">Authorization</span></span>  | <span data-ttu-id="311b1-131">string</span><span class="sxs-lookup"><span data-stu-id="311b1-131">string</span></span>  | <span data-ttu-id="311b1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="311b1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="311b1-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="311b1-134">Content-Type</span></span> | <span data-ttu-id="311b1-135">string</span><span class="sxs-lookup"><span data-stu-id="311b1-135">string</span></span>  | <span data-ttu-id="311b1-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="311b1-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="311b1-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="311b1-138">Request body</span></span>
<span data-ttu-id="311b1-139">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="311b1-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="311b1-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="311b1-140">Parameter</span></span>    | <span data-ttu-id="311b1-141">Typ</span><span class="sxs-lookup"><span data-stu-id="311b1-141">Type</span></span>   |<span data-ttu-id="311b1-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="311b1-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="311b1-143">comment</span><span class="sxs-lookup"><span data-stu-id="311b1-143">comment</span></span>|<span data-ttu-id="311b1-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="311b1-144">String</span></span>|<span data-ttu-id="311b1-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="311b1-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="311b1-147">message</span><span class="sxs-lookup"><span data-stu-id="311b1-147">message</span></span>|[<span data-ttu-id="311b1-148">message</span><span class="sxs-lookup"><span data-stu-id="311b1-148">message</span></span>](../resources/message.md)|<span data-ttu-id="311b1-149">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="311b1-149">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="311b1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="311b1-150">Response</span></span>

<span data-ttu-id="311b1-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="311b1-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="311b1-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="311b1-153">Example</span></span>
<span data-ttu-id="311b1-154">Das folgende Beispiel enthält einen Kommentar und fügt eine Anlage, die allen Antworten-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="311b1-154">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="311b1-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="311b1-155">Request</span></span>
<span data-ttu-id="311b1-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="311b1-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a><span data-ttu-id="311b1-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="311b1-157">Response</span></span>
<span data-ttu-id="311b1-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="311b1-158">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
