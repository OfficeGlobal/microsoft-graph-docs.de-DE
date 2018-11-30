---
title: 'message: forward'
description: 'Weiterleiten einer Nachricht, einen Kommentar hinzufügen oder Ändern von aktualisierbaren Eigenschaften  '
ms.openlocfilehash: 3edb96a90c99f1bc9eb2d8499e9cda83774a7ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065750"
---
# <a name="message-forward"></a><span data-ttu-id="dbe51-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="dbe51-103">message: forward</span></span>

> <span data-ttu-id="dbe51-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbe51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbe51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbe51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbe51-106">Weiterleiten einer Nachricht, einen Kommentar hinzufügen oder Ändern von aktualisierbaren Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbe51-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="dbe51-107">Rufen Sie alle in einem **Weiterleiten** .</span><span class="sxs-lookup"><span data-stu-id="dbe51-107">all in one **forward** call.</span></span> <span data-ttu-id="dbe51-108">Die Nachricht wird im Ordner "Gesendete Elemente" gespeichert.</span><span class="sxs-lookup"><span data-stu-id="dbe51-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="dbe51-109">Alternativ können Sie zunächst [den Entwurf Weiterleiten einer Nachricht erstellen](../api/message-createforward.md) zum Einschließen eines Kommentars oder aktualisieren Sie alle Nachrichteneigenschaften, und klicken Sie dann den Entwurf einer Nachricht [Senden](../api/message-send.md) .</span><span class="sxs-lookup"><span data-stu-id="dbe51-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="dbe51-110">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="dbe51-110">**Note**</span></span>

- <span data-ttu-id="dbe51-111">Sie können einen Kommentar oder die **Body** -Eigenschaft des angeben die `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="dbe51-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="dbe51-112">Beide angeben, gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="dbe51-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="dbe51-113">Geben Sie entweder die `toRecipients` Parameter oder die **ToRecipients** -Eigenschaft des der `message` Parameter.</span><span class="sxs-lookup"><span data-stu-id="dbe51-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="dbe51-114">Beide angeben oder keine Angabe gibt einen HTTP 400 Ungültige Anforderung Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="dbe51-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe51-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dbe51-115">Permissions</span></span>
<span data-ttu-id="dbe51-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe51-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe51-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dbe51-118">Permission type</span></span>      | <span data-ttu-id="dbe51-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dbe51-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe51-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dbe51-120">Delegated (work or school account)</span></span> | <span data-ttu-id="dbe51-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dbe51-121">Mail.Send</span></span>    |
|<span data-ttu-id="dbe51-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dbe51-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbe51-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dbe51-123">Mail.Send</span></span>    |
|<span data-ttu-id="dbe51-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dbe51-124">Application</span></span> | <span data-ttu-id="dbe51-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dbe51-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe51-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbe51-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="dbe51-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dbe51-127">Request headers</span></span>
| <span data-ttu-id="dbe51-128">Name</span><span class="sxs-lookup"><span data-stu-id="dbe51-128">Name</span></span>       | <span data-ttu-id="dbe51-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dbe51-129">Type</span></span> | <span data-ttu-id="dbe51-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbe51-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbe51-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe51-131">Authorization</span></span>  | <span data-ttu-id="dbe51-132">string</span><span class="sxs-lookup"><span data-stu-id="dbe51-132">string</span></span>  | <span data-ttu-id="dbe51-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dbe51-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbe51-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbe51-135">Content-Type</span></span> | <span data-ttu-id="dbe51-136">string</span><span class="sxs-lookup"><span data-stu-id="dbe51-136">string</span></span>  | <span data-ttu-id="dbe51-p107">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dbe51-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbe51-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dbe51-139">Request body</span></span>
<span data-ttu-id="dbe51-140">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="dbe51-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbe51-141">Parameter</span><span class="sxs-lookup"><span data-stu-id="dbe51-141">Parameter</span></span>    | <span data-ttu-id="dbe51-142">Typ</span><span class="sxs-lookup"><span data-stu-id="dbe51-142">Type</span></span>   |<span data-ttu-id="dbe51-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbe51-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbe51-144">comment</span><span class="sxs-lookup"><span data-stu-id="dbe51-144">comment</span></span>|<span data-ttu-id="dbe51-145">String</span><span class="sxs-lookup"><span data-stu-id="dbe51-145">String</span></span>|<span data-ttu-id="dbe51-p108">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="dbe51-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="dbe51-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="dbe51-148">toRecipients</span></span>|<span data-ttu-id="dbe51-149">[recipient](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dbe51-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="dbe51-150">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="dbe51-150">The list of recipients.</span></span>|
|<span data-ttu-id="dbe51-151">message</span><span class="sxs-lookup"><span data-stu-id="dbe51-151">message</span></span>|[<span data-ttu-id="dbe51-152">Nachricht</span><span class="sxs-lookup"><span data-stu-id="dbe51-152">message</span></span>](../resources/message.md)|<span data-ttu-id="dbe51-153">Alle schreibbaren Eigenschaften, die in der Antwortnachricht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="dbe51-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="dbe51-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbe51-154">Response</span></span>

<span data-ttu-id="dbe51-p109">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dbe51-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe51-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dbe51-157">Example</span></span>
<span data-ttu-id="dbe51-158">Im folgenden Beispiel wird die **IsDeliveryReceiptRequested** -Eigenschaft auf True festgelegt, wird ein Kommentar hinzugefügt und leitet die Nachricht weiter.</span><span class="sxs-lookup"><span data-stu-id="dbe51-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="dbe51-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dbe51-159">Request</span></span>
<span data-ttu-id="dbe51-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dbe51-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dbe51-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="dbe51-161">Response</span></span>
<span data-ttu-id="dbe51-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dbe51-162">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->