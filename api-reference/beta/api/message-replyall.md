---
title: 'message: replyAll'
description: 'Antworten Sie an alle Empfänger einer Nachricht durch einen Kommentar angeben und keine aktualisierbaren Eigenschaften ändern '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 05f552676400196aed275c32020bcdf5211d0e31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528613"
---
# <a name="message-replyall"></a><span data-ttu-id="cfaa4-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="cfaa4-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfaa4-104">Antworten Sie an alle Empfänger einer Nachricht durch einen Kommentar angeben und ändern keine aktualisierbaren Eigenschaften für die Antwort, die alle mithilfe der **ReplyAll** -Methode.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="cfaa4-105">Die Nachricht wird im Ordner "Gesendete Elemente" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="cfaa4-106">Alternativ können Sie zunächst [Erstellen Sie eine Entwurf allen Antworten - Nachricht](../api/message-createreplyall.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Eigenschaften der Nachricht, und die Antwort zu [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="cfaa4-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="cfaa4-107">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="cfaa4-107">**Note**</span></span>

- <span data-ttu-id="cfaa4-108">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="cfaa4-109">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="cfaa4-110">Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie senden Sie die Antwort an die Empfänger in der</span><span class="sxs-lookup"><span data-stu-id="cfaa4-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="cfaa4-111">**ReplyTo** und **ToRecipients** -Eigenschaften, und nicht die Empfänger in den Eigenschaften **von** und **ToRecipients** .</span><span class="sxs-lookup"><span data-stu-id="cfaa4-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="cfaa4-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cfaa4-112">Permissions</span></span>
<span data-ttu-id="cfaa4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfaa4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfaa4-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfaa4-115">Permission type</span></span>      | <span data-ttu-id="cfaa4-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfaa4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfaa4-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfaa4-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cfaa4-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cfaa4-118">Mail.Send</span></span>    |
|<span data-ttu-id="cfaa4-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfaa4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfaa4-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cfaa4-120">Mail.Send</span></span>    |
|<span data-ttu-id="cfaa4-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfaa4-121">Application</span></span> | <span data-ttu-id="cfaa4-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cfaa4-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfaa4-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfaa4-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="cfaa4-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfaa4-124">Request headers</span></span>
| <span data-ttu-id="cfaa4-125">Name</span><span class="sxs-lookup"><span data-stu-id="cfaa4-125">Name</span></span>       | <span data-ttu-id="cfaa4-126">Typ</span><span class="sxs-lookup"><span data-stu-id="cfaa4-126">Type</span></span> | <span data-ttu-id="cfaa4-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfaa4-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfaa4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfaa4-128">Authorization</span></span>  | <span data-ttu-id="cfaa4-129">string</span><span class="sxs-lookup"><span data-stu-id="cfaa4-129">string</span></span>  | <span data-ttu-id="cfaa4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfaa4-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfaa4-132">Content-Type</span></span> | <span data-ttu-id="cfaa4-133">string</span><span class="sxs-lookup"><span data-stu-id="cfaa4-133">string</span></span>  | <span data-ttu-id="cfaa4-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfaa4-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfaa4-136">Request body</span></span>
<span data-ttu-id="cfaa4-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cfaa4-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="cfaa4-138">Parameter</span></span>    | <span data-ttu-id="cfaa4-139">Typ</span><span class="sxs-lookup"><span data-stu-id="cfaa4-139">Type</span></span>   |<span data-ttu-id="cfaa4-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfaa4-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfaa4-141">comment</span><span class="sxs-lookup"><span data-stu-id="cfaa4-141">comment</span></span>|<span data-ttu-id="cfaa4-142">String</span><span class="sxs-lookup"><span data-stu-id="cfaa4-142">String</span></span>|<span data-ttu-id="cfaa4-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="cfaa4-145">message</span><span class="sxs-lookup"><span data-stu-id="cfaa4-145">message</span></span>|[<span data-ttu-id="cfaa4-146">Nachricht</span><span class="sxs-lookup"><span data-stu-id="cfaa4-146">message</span></span>](../resources/message.md)|<span data-ttu-id="cfaa4-147">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="cfaa4-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfaa4-148">Response</span></span>

<span data-ttu-id="cfaa4-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfaa4-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfaa4-151">Example</span></span>
<span data-ttu-id="cfaa4-152">Das folgende Beispiel enthält einen Kommentar und fügt eine Anlage, die allen Antworten-Nachricht.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="cfaa4-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfaa4-153">Request</span></span>
<span data-ttu-id="cfaa4-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-154">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="cfaa4-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfaa4-155">Response</span></span>
<span data-ttu-id="cfaa4-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cfaa4-156">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
