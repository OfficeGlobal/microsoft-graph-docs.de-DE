---
title: 'message: forward'
description: Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 12409685e21b338a86b392f32449b006a0e958f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960546"
---
# <a name="message-forward"></a><span data-ttu-id="9cdee-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="9cdee-104">message: forward</span></span>

<span data-ttu-id="9cdee-p102">Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="9cdee-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cdee-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9cdee-107">Permissions</span></span>
<span data-ttu-id="9cdee-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cdee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cdee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9cdee-110">Permission type</span></span>      | <span data-ttu-id="9cdee-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9cdee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cdee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9cdee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9cdee-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9cdee-113">Mail.Send</span></span>    |
|<span data-ttu-id="9cdee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9cdee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cdee-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9cdee-115">Mail.Send</span></span>    |
|<span data-ttu-id="9cdee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9cdee-116">Application</span></span> | <span data-ttu-id="9cdee-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9cdee-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cdee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cdee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="9cdee-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9cdee-119">Request headers</span></span>
| <span data-ttu-id="9cdee-120">Name</span><span class="sxs-lookup"><span data-stu-id="9cdee-120">Name</span></span>       | <span data-ttu-id="9cdee-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9cdee-121">Type</span></span> | <span data-ttu-id="9cdee-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cdee-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cdee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cdee-123">Authorization</span></span>  | <span data-ttu-id="9cdee-124">string</span><span class="sxs-lookup"><span data-stu-id="9cdee-124">string</span></span>  | <span data-ttu-id="9cdee-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9cdee-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cdee-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cdee-127">Content-Type</span></span> | <span data-ttu-id="9cdee-128">string</span><span class="sxs-lookup"><span data-stu-id="9cdee-128">string</span></span>  | <span data-ttu-id="9cdee-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9cdee-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cdee-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9cdee-131">Request body</span></span>
<span data-ttu-id="9cdee-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9cdee-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9cdee-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="9cdee-133">Parameter</span></span>    | <span data-ttu-id="9cdee-134">Typ</span><span class="sxs-lookup"><span data-stu-id="9cdee-134">Type</span></span>   |<span data-ttu-id="9cdee-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cdee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cdee-136">comment</span><span class="sxs-lookup"><span data-stu-id="9cdee-136">comment</span></span>|<span data-ttu-id="9cdee-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cdee-137">String</span></span>|<span data-ttu-id="9cdee-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="9cdee-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="9cdee-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="9cdee-140">toRecipients</span></span>|<span data-ttu-id="9cdee-141">[Recipient collection](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9cdee-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="9cdee-142">Die Liste der Empfänger.</span><span class="sxs-lookup"><span data-stu-id="9cdee-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="9cdee-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cdee-143">Response</span></span>

<span data-ttu-id="9cdee-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cdee-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cdee-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cdee-146">Example</span></span>
<span data-ttu-id="9cdee-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9cdee-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9cdee-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cdee-148">Request</span></span>
<span data-ttu-id="9cdee-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cdee-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9cdee-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cdee-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9cdee-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cdee-151">Response</span></span>
<span data-ttu-id="9cdee-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9cdee-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
