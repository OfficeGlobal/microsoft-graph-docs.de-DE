---
title: 'message: createReplyAll'
description: 'Erstellen Sie ein Entwurfs oder eine allen Antworten-Nachricht enthalten einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7f0b2631f02a94a7627e96e24308b135d70d20e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922172"
---
# <a name="message-createreplyall"></a><span data-ttu-id="7a217-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="7a217-103">message: createReplyAll</span></span>

> <span data-ttu-id="7a217-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a217-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a217-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a217-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a217-p102">Erstellt einen Entwurf einer Antwortnachricht an alle Empfänger, um in einem **createReplyAll**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).</span><span class="sxs-lookup"><span data-stu-id="7a217-p102">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="7a217-108">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="7a217-108">**Note**</span></span>

- <span data-ttu-id="7a217-109">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="7a217-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7a217-110">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="7a217-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7a217-111">Wenn die **ReplyTo** -Eigenschaft angegeben wird, in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), sollten Sie senden Sie die Antwort an die Empfänger in der</span><span class="sxs-lookup"><span data-stu-id="7a217-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="7a217-112">**ReplyTo** und **ToRecipients** -Eigenschaften, und nicht die Empfänger in den Eigenschaften **von** und **ToRecipients** .</span><span class="sxs-lookup"><span data-stu-id="7a217-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7a217-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a217-113">Permissions</span></span>
<span data-ttu-id="7a217-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a217-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a217-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a217-116">Permission type</span></span>      | <span data-ttu-id="7a217-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a217-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a217-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a217-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7a217-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a217-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7a217-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a217-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a217-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a217-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7a217-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a217-122">Application</span></span> | <span data-ttu-id="7a217-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a217-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a217-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a217-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="7a217-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a217-125">Request headers</span></span>
| <span data-ttu-id="7a217-126">Name</span><span class="sxs-lookup"><span data-stu-id="7a217-126">Name</span></span>       | <span data-ttu-id="7a217-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7a217-127">Type</span></span> | <span data-ttu-id="7a217-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a217-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7a217-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a217-129">Authorization</span></span>  | <span data-ttu-id="7a217-130">string</span><span class="sxs-lookup"><span data-stu-id="7a217-130">string</span></span>  | <span data-ttu-id="7a217-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a217-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a217-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a217-133">Content-Type</span></span> | <span data-ttu-id="7a217-134">string</span><span class="sxs-lookup"><span data-stu-id="7a217-134">string</span></span>  | <span data-ttu-id="7a217-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a217-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a217-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a217-137">Request body</span></span>
<span data-ttu-id="7a217-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7a217-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7a217-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="7a217-139">Parameter</span></span>    | <span data-ttu-id="7a217-140">Typ</span><span class="sxs-lookup"><span data-stu-id="7a217-140">Type</span></span>   |<span data-ttu-id="7a217-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a217-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a217-142">comment</span><span class="sxs-lookup"><span data-stu-id="7a217-142">comment</span></span>|<span data-ttu-id="7a217-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a217-143">String</span></span>|<span data-ttu-id="7a217-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="7a217-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7a217-146">message</span><span class="sxs-lookup"><span data-stu-id="7a217-146">message</span></span>|[<span data-ttu-id="7a217-147">message</span><span class="sxs-lookup"><span data-stu-id="7a217-147">message</span></span>](../resources/message.md)|<span data-ttu-id="7a217-148">Alle schreibbaren Eigenschaften, in die allen Antworten-Nachricht zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7a217-148">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="7a217-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a217-149">Response</span></span>

<span data-ttu-id="7a217-150">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a217-150">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a217-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a217-151">Example</span></span>
<span data-ttu-id="7a217-152">Im folgenden Beispiel wird einen Entwurf, um alle Antworten erstellt und eine Anlage und Kommentar in ein **CreateReplyAll** Aufruf hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="7a217-152">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="7a217-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a217-153">Request</span></span>
<span data-ttu-id="7a217-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a217-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
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
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```

##### <a name="response"></a><span data-ttu-id="7a217-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a217-155">Response</span></span>
<span data-ttu-id="7a217-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a217-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
