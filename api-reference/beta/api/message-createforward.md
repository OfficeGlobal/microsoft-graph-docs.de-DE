---
title: 'message: createForward'
description: 'Erstellen Sie eine Nachricht der Entwurf forward eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2c750ac0dd8f6a6226161701950bd879025f9641
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519528"
---
# <a name="message-createforward"></a><span data-ttu-id="5f1e0-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="5f1e0-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f1e0-104">Erstellen Sie eine Nachricht der Entwurf forward eingeschlossen einen Kommentar oder aktualisieren Sie die Nachrichteneigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f1e0-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="5f1e0-105">Rufen Sie alle in einem **CreateForward** auf.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-105">all in one **createForward** call.</span></span> <span data-ttu-id="5f1e0-106">Anschließend können Sie den Entwurf einer Nachricht [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="5f1e0-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="5f1e0-107">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="5f1e0-107">**Note**</span></span>

- <span data-ttu-id="5f1e0-108">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="5f1e0-109">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5f1e0-110">Geben Sie entweder die `toRecipients` Parameter oder die **ToRecipients** -Eigenschaft des der `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="5f1e0-111">Beide angeben oder keine Angabe gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1e0-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5f1e0-112">Permissions</span></span>
<span data-ttu-id="5f1e0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1e0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f1e0-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f1e0-115">Permission type</span></span>      | <span data-ttu-id="5f1e0-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f1e0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f1e0-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f1e0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5f1e0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1e0-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f1e0-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f1e0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f1e0-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1e0-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f1e0-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f1e0-121">Application</span></span> | <span data-ttu-id="5f1e0-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1e0-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f1e0-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f1e0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="5f1e0-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f1e0-124">Request headers</span></span>
| <span data-ttu-id="5f1e0-125">Name</span><span class="sxs-lookup"><span data-stu-id="5f1e0-125">Name</span></span>       | <span data-ttu-id="5f1e0-126">Typ</span><span class="sxs-lookup"><span data-stu-id="5f1e0-126">Type</span></span> | <span data-ttu-id="5f1e0-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f1e0-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f1e0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f1e0-128">Authorization</span></span>  | <span data-ttu-id="5f1e0-129">string</span><span class="sxs-lookup"><span data-stu-id="5f1e0-129">string</span></span>  | <span data-ttu-id="5f1e0-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f1e0-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f1e0-132">Content-Type</span></span> | <span data-ttu-id="5f1e0-133">string</span><span class="sxs-lookup"><span data-stu-id="5f1e0-133">string</span></span>  | <span data-ttu-id="5f1e0-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f1e0-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f1e0-136">Request body</span></span>
<span data-ttu-id="5f1e0-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f1e0-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="5f1e0-138">Parameter</span></span>    | <span data-ttu-id="5f1e0-139">Typ</span><span class="sxs-lookup"><span data-stu-id="5f1e0-139">Type</span></span>   |<span data-ttu-id="5f1e0-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f1e0-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f1e0-141">comment</span><span class="sxs-lookup"><span data-stu-id="5f1e0-141">comment</span></span>|<span data-ttu-id="5f1e0-142">String</span><span class="sxs-lookup"><span data-stu-id="5f1e0-142">String</span></span>|<span data-ttu-id="5f1e0-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="5f1e0-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5f1e0-145">toRecipients</span></span>|<span data-ttu-id="5f1e0-146">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="5f1e0-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="5f1e0-147">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-147">The list of recipients.</span></span>|
|<span data-ttu-id="5f1e0-148">message</span><span class="sxs-lookup"><span data-stu-id="5f1e0-148">message</span></span>|[<span data-ttu-id="5f1e0-149">Nachricht</span><span class="sxs-lookup"><span data-stu-id="5f1e0-149">message</span></span>](../resources/message.md)|<span data-ttu-id="5f1e0-150">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="5f1e0-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f1e0-151">Response</span></span>

<span data-ttu-id="5f1e0-152">Bei erfolgreicher Ausführung der Methode werden der Antwortcode `201 Created` und das [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f1e0-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f1e0-153">Example</span></span>
<span data-ttu-id="5f1e0-154">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f1e0-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f1e0-155">Request</span></span>
<span data-ttu-id="5f1e0-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5f1e0-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f1e0-157">Response</span></span>
<span data-ttu-id="5f1e0-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f1e0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
