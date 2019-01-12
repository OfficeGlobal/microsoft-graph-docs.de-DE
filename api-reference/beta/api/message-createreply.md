---
title: 'message: createReply'
description: 'Erstellen Sie ein Entwurfs oder eine Antwortnachricht eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 27e6aabe05cb732cd40242f3c17c822c920c062e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943739"
---
# <a name="message-createreply"></a><span data-ttu-id="0a145-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="0a145-103">message: createReply</span></span>

> <span data-ttu-id="0a145-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a145-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a145-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a145-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a145-p102">Erstellt einen Entwurf einer Antwortnachricht, um in einem **createReply**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).</span><span class="sxs-lookup"><span data-stu-id="0a145-p102">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="0a145-108">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="0a145-108">**Note**</span></span>

- <span data-ttu-id="0a145-109">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="0a145-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="0a145-110">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="0a145-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="0a145-111">Wenn **ReplyTo** in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) angegeben wird, sollten Sie die Antwort an den Empfänger in **ReplyTo**und nicht die Empfänger in **aus**senden.</span><span class="sxs-lookup"><span data-stu-id="0a145-111">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0a145-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a145-112">Permissions</span></span>
<span data-ttu-id="0a145-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a145-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a145-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a145-115">Permission type</span></span>      | <span data-ttu-id="0a145-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a145-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a145-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a145-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0a145-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a145-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0a145-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a145-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a145-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a145-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0a145-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a145-121">Application</span></span> | <span data-ttu-id="0a145-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a145-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a145-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a145-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="0a145-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a145-124">Request headers</span></span>
| <span data-ttu-id="0a145-125">Name</span><span class="sxs-lookup"><span data-stu-id="0a145-125">Name</span></span>       | <span data-ttu-id="0a145-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0a145-126">Type</span></span> | <span data-ttu-id="0a145-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a145-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a145-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a145-128">Authorization</span></span>  | <span data-ttu-id="0a145-129">string</span><span class="sxs-lookup"><span data-stu-id="0a145-129">string</span></span>  | <span data-ttu-id="0a145-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a145-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a145-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a145-132">Content-Type</span></span> | <span data-ttu-id="0a145-133">string</span><span class="sxs-lookup"><span data-stu-id="0a145-133">string</span></span>  | <span data-ttu-id="0a145-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a145-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a145-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a145-136">Request body</span></span>
<span data-ttu-id="0a145-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0a145-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a145-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="0a145-138">Parameter</span></span>    | <span data-ttu-id="0a145-139">Typ</span><span class="sxs-lookup"><span data-stu-id="0a145-139">Type</span></span>   |<span data-ttu-id="0a145-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a145-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a145-141">comment</span><span class="sxs-lookup"><span data-stu-id="0a145-141">comment</span></span>|<span data-ttu-id="0a145-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a145-142">String</span></span>|<span data-ttu-id="0a145-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="0a145-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="0a145-145">message</span><span class="sxs-lookup"><span data-stu-id="0a145-145">message</span></span>|[<span data-ttu-id="0a145-146">message</span><span class="sxs-lookup"><span data-stu-id="0a145-146">message</span></span>](../resources/message.md)|<span data-ttu-id="0a145-147">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0a145-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="0a145-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a145-148">Response</span></span>

<span data-ttu-id="0a145-149">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a145-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a145-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a145-150">Example</span></span>
<span data-ttu-id="0a145-151">Im folgende Beispiel erstellt einen Entwurf Antwort, fügt einen Kommentar und einem Empfänger im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a145-151">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="0a145-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a145-152">Request</span></span>
<span data-ttu-id="0a145-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a145-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
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
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```

##### <a name="response"></a><span data-ttu-id="0a145-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a145-154">Response</span></span>
<span data-ttu-id="0a145-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a145-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
