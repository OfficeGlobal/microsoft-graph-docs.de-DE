---
title: 'message: createForward'
description: 'Erstellen Sie eine Nachricht der Entwurf forward eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften  '
ms.openlocfilehash: 8e7710871000222d1281a274ee270885097351f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062084"
---
# <a name="message-createforward"></a><span data-ttu-id="10614-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="10614-103">message: createForward</span></span>

> <span data-ttu-id="10614-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10614-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10614-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10614-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10614-106">Erstellen Sie eine Nachricht der Entwurf forward eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften</span><span class="sxs-lookup"><span data-stu-id="10614-106">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="10614-107">Rufen Sie alle in einem **CreateForward** auf.</span><span class="sxs-lookup"><span data-stu-id="10614-107">all in one **createForward** call.</span></span> <span data-ttu-id="10614-108">Anschließend können Sie den Entwurf einer Nachricht [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="10614-108">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="10614-109">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="10614-109">**Note**</span></span>

- <span data-ttu-id="10614-110">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="10614-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="10614-111">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="10614-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="10614-112">Geben Sie entweder die `toRecipients` Parameter oder die **ToRecipients** -Eigenschaft des der `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="10614-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="10614-113">Beide angeben oder keine Angabe gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="10614-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="10614-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10614-114">Permissions</span></span>
<span data-ttu-id="10614-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10614-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10614-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10614-117">Permission type</span></span>      | <span data-ttu-id="10614-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10614-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10614-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10614-119">Delegated (work or school account)</span></span> | <span data-ttu-id="10614-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10614-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10614-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10614-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10614-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10614-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="10614-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10614-123">Application</span></span> | <span data-ttu-id="10614-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10614-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10614-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10614-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="10614-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10614-126">Request headers</span></span>
| <span data-ttu-id="10614-127">Name</span><span class="sxs-lookup"><span data-stu-id="10614-127">Name</span></span>       | <span data-ttu-id="10614-128">Typ</span><span class="sxs-lookup"><span data-stu-id="10614-128">Type</span></span> | <span data-ttu-id="10614-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10614-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10614-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="10614-130">Authorization</span></span>  | <span data-ttu-id="10614-131">string</span><span class="sxs-lookup"><span data-stu-id="10614-131">string</span></span>  | <span data-ttu-id="10614-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10614-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10614-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10614-134">Content-Type</span></span> | <span data-ttu-id="10614-135">string</span><span class="sxs-lookup"><span data-stu-id="10614-135">string</span></span>  | <span data-ttu-id="10614-p107">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10614-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10614-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10614-138">Request body</span></span>
<span data-ttu-id="10614-139">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="10614-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10614-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="10614-140">Parameter</span></span>    | <span data-ttu-id="10614-141">Typ</span><span class="sxs-lookup"><span data-stu-id="10614-141">Type</span></span>   |<span data-ttu-id="10614-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10614-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10614-143">comment</span><span class="sxs-lookup"><span data-stu-id="10614-143">comment</span></span>|<span data-ttu-id="10614-144">String</span><span class="sxs-lookup"><span data-stu-id="10614-144">String</span></span>|<span data-ttu-id="10614-p108">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="10614-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="10614-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="10614-147">toRecipients</span></span>|<span data-ttu-id="10614-148">[recipient](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10614-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="10614-149">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="10614-149">The list of recipients.</span></span>|
|<span data-ttu-id="10614-150">message</span><span class="sxs-lookup"><span data-stu-id="10614-150">message</span></span>|[<span data-ttu-id="10614-151">Nachricht</span><span class="sxs-lookup"><span data-stu-id="10614-151">message</span></span>](../resources/message.md)|<span data-ttu-id="10614-152">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="10614-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="10614-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="10614-153">Response</span></span>

<span data-ttu-id="10614-154">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10614-154">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10614-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10614-155">Example</span></span>
<span data-ttu-id="10614-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="10614-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="10614-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10614-157">Request</span></span>
<span data-ttu-id="10614-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10614-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```

##### <a name="response"></a><span data-ttu-id="10614-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="10614-159">Response</span></span>
<span data-ttu-id="10614-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10614-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->