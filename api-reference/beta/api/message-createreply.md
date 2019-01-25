---
title: 'message: createReply'
description: 'Erstellen Sie ein Entwurfs oder eine Antwortnachricht eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 112db29116625da1c154783eee840c7a69b5ebfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526837"
---
# <a name="message-createreply"></a><span data-ttu-id="af8d9-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="af8d9-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af8d9-p101">Erstellt einen Entwurf einer Antwortnachricht, um in einem **createReply**-Aufruf einen Kommentar einzuschließen oder Nachrichteneigenschaften zu aktualisieren. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).</span><span class="sxs-lookup"><span data-stu-id="af8d9-p101">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call. You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="af8d9-106">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="af8d9-106">**Note**</span></span>

- <span data-ttu-id="af8d9-107">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="af8d9-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="af8d9-108">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="af8d9-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="af8d9-109">Wenn **ReplyTo** in der ursprünglichen Nachricht pro Internet-Nachrichtenformat ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)) angegeben wird, sollten Sie die Antwort an den Empfänger in **ReplyTo**und nicht die Empfänger in **aus**senden.</span><span class="sxs-lookup"><span data-stu-id="af8d9-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="af8d9-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="af8d9-110">Permissions</span></span>
<span data-ttu-id="af8d9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af8d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8d9-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af8d9-113">Permission type</span></span>      | <span data-ttu-id="af8d9-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af8d9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8d9-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af8d9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="af8d9-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8d9-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="af8d9-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af8d9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8d9-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8d9-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="af8d9-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af8d9-119">Application</span></span> | <span data-ttu-id="af8d9-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8d9-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8d9-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af8d9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="af8d9-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af8d9-122">Request headers</span></span>
| <span data-ttu-id="af8d9-123">Name</span><span class="sxs-lookup"><span data-stu-id="af8d9-123">Name</span></span>       | <span data-ttu-id="af8d9-124">Typ</span><span class="sxs-lookup"><span data-stu-id="af8d9-124">Type</span></span> | <span data-ttu-id="af8d9-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af8d9-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af8d9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="af8d9-126">Authorization</span></span>  | <span data-ttu-id="af8d9-127">string</span><span class="sxs-lookup"><span data-stu-id="af8d9-127">string</span></span>  | <span data-ttu-id="af8d9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="af8d9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af8d9-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af8d9-130">Content-Type</span></span> | <span data-ttu-id="af8d9-131">string</span><span class="sxs-lookup"><span data-stu-id="af8d9-131">string</span></span>  | <span data-ttu-id="af8d9-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="af8d9-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af8d9-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af8d9-134">Request body</span></span>
<span data-ttu-id="af8d9-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="af8d9-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af8d9-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="af8d9-136">Parameter</span></span>    | <span data-ttu-id="af8d9-137">Typ</span><span class="sxs-lookup"><span data-stu-id="af8d9-137">Type</span></span>   |<span data-ttu-id="af8d9-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af8d9-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af8d9-139">comment</span><span class="sxs-lookup"><span data-stu-id="af8d9-139">comment</span></span>|<span data-ttu-id="af8d9-140">String</span><span class="sxs-lookup"><span data-stu-id="af8d9-140">String</span></span>|<span data-ttu-id="af8d9-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="af8d9-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="af8d9-143">message</span><span class="sxs-lookup"><span data-stu-id="af8d9-143">message</span></span>|[<span data-ttu-id="af8d9-144">Nachricht</span><span class="sxs-lookup"><span data-stu-id="af8d9-144">message</span></span>](../resources/message.md)|<span data-ttu-id="af8d9-145">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="af8d9-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="af8d9-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="af8d9-146">Response</span></span>

<span data-ttu-id="af8d9-147">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af8d9-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8d9-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af8d9-148">Example</span></span>
<span data-ttu-id="af8d9-149">Im folgende Beispiel erstellt einen Entwurf Antwort, fügt einen Kommentar und einem Empfänger im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af8d9-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="af8d9-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af8d9-150">Request</span></span>
<span data-ttu-id="af8d9-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af8d9-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="af8d9-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="af8d9-152">Response</span></span>
<span data-ttu-id="af8d9-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af8d9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createreply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
