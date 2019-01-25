---
title: 'message: forward'
description: 'Weiterleiten einer Nachricht, einen Kommentar hinzufügen oder Ändern von aktualisierbaren Eigenschaften  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed3d51c28e6fe0404b5cb26fb17f6d8ed3bba212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508888"
---
# <a name="message-forward"></a><span data-ttu-id="090b4-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="090b4-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090b4-104">Weiterleiten einer Nachricht, einen Kommentar hinzufügen oder Ändern von aktualisierbaren Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="090b4-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="090b4-105">Rufen Sie alle in einem **Weiterleiten** .</span><span class="sxs-lookup"><span data-stu-id="090b4-105">all in one **forward** call.</span></span> <span data-ttu-id="090b4-106">Die Nachricht wird im Ordner "Gesendete Elemente" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="090b4-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="090b4-107">Alternativ können Sie zunächst [den Entwurf Weiterleiten einer Nachricht erstellen](../api/message-createforward.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Nachrichteneigenschaften, und klicken Sie dann den Entwurf einer Nachricht [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="090b4-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="090b4-108">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="090b4-108">**Note**</span></span>

- <span data-ttu-id="090b4-109">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="090b4-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="090b4-110">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="090b4-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="090b4-111">Geben Sie entweder die `toRecipients` Parameter oder die **ToRecipients** -Eigenschaft des der `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="090b4-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="090b4-112">Beide angeben oder keine Angabe gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="090b4-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="090b4-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="090b4-113">Permissions</span></span>
<span data-ttu-id="090b4-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="090b4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="090b4-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="090b4-116">Permission type</span></span>      | <span data-ttu-id="090b4-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="090b4-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="090b4-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="090b4-118">Delegated (work or school account)</span></span> | <span data-ttu-id="090b4-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="090b4-119">Mail.Send</span></span>    |
|<span data-ttu-id="090b4-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="090b4-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="090b4-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="090b4-121">Mail.Send</span></span>    |
|<span data-ttu-id="090b4-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="090b4-122">Application</span></span> | <span data-ttu-id="090b4-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="090b4-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="090b4-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="090b4-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="090b4-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="090b4-125">Request headers</span></span>
| <span data-ttu-id="090b4-126">Name</span><span class="sxs-lookup"><span data-stu-id="090b4-126">Name</span></span>       | <span data-ttu-id="090b4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="090b4-127">Type</span></span> | <span data-ttu-id="090b4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="090b4-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="090b4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="090b4-129">Authorization</span></span>  | <span data-ttu-id="090b4-130">string</span><span class="sxs-lookup"><span data-stu-id="090b4-130">string</span></span>  | <span data-ttu-id="090b4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="090b4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="090b4-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="090b4-133">Content-Type</span></span> | <span data-ttu-id="090b4-134">string</span><span class="sxs-lookup"><span data-stu-id="090b4-134">string</span></span>  | <span data-ttu-id="090b4-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="090b4-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="090b4-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="090b4-137">Request body</span></span>
<span data-ttu-id="090b4-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="090b4-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="090b4-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="090b4-139">Parameter</span></span>    | <span data-ttu-id="090b4-140">Typ</span><span class="sxs-lookup"><span data-stu-id="090b4-140">Type</span></span>   |<span data-ttu-id="090b4-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="090b4-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="090b4-142">comment</span><span class="sxs-lookup"><span data-stu-id="090b4-142">comment</span></span>|<span data-ttu-id="090b4-143">String</span><span class="sxs-lookup"><span data-stu-id="090b4-143">String</span></span>|<span data-ttu-id="090b4-p107">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="090b4-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="090b4-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="090b4-146">toRecipients</span></span>|<span data-ttu-id="090b4-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="090b4-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="090b4-148">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="090b4-148">The list of recipients.</span></span>|
|<span data-ttu-id="090b4-149">message</span><span class="sxs-lookup"><span data-stu-id="090b4-149">message</span></span>|[<span data-ttu-id="090b4-150">Nachricht</span><span class="sxs-lookup"><span data-stu-id="090b4-150">message</span></span>](../resources/message.md)|<span data-ttu-id="090b4-151">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="090b4-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="090b4-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="090b4-152">Response</span></span>

<span data-ttu-id="090b4-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="090b4-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="090b4-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="090b4-155">Example</span></span>
<span data-ttu-id="090b4-156">Im folgenden Beispiel wird die **IsDeliveryReceiptRequested** -Eigenschaft auf True festgelegt, wird ein Kommentar hinzugefügt und leitet die Nachricht weiter.</span><span class="sxs-lookup"><span data-stu-id="090b4-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="090b4-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="090b4-157">Request</span></span>
<span data-ttu-id="090b4-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="090b4-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
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
  "comment": "Dana, just want to make sure you get this." 
}
```

##### <a name="response"></a><span data-ttu-id="090b4-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="090b4-159">Response</span></span>
<span data-ttu-id="090b4-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="090b4-160">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
