---
title: 'message: reply'
description: Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1aacac847295926562036a65007cac1f542f50fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961309"
---
# <a name="message-reply"></a><span data-ttu-id="8acf2-104">message: reply</span><span class="sxs-lookup"><span data-stu-id="8acf2-104">message: reply</span></span>

<span data-ttu-id="8acf2-p102">Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="8acf2-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8acf2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8acf2-107">Permissions</span></span>
<span data-ttu-id="8acf2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8acf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8acf2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8acf2-110">Permission type</span></span>      | <span data-ttu-id="8acf2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8acf2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8acf2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8acf2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8acf2-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8acf2-113">Mail.Send</span></span>    |
|<span data-ttu-id="8acf2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8acf2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8acf2-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8acf2-115">Mail.Send</span></span>    |
|<span data-ttu-id="8acf2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8acf2-116">Application</span></span> | <span data-ttu-id="8acf2-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8acf2-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8acf2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8acf2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="8acf2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8acf2-119">Request headers</span></span>
| <span data-ttu-id="8acf2-120">Name</span><span class="sxs-lookup"><span data-stu-id="8acf2-120">Name</span></span>       | <span data-ttu-id="8acf2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8acf2-121">Type</span></span> | <span data-ttu-id="8acf2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8acf2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8acf2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8acf2-123">Authorization</span></span>  | <span data-ttu-id="8acf2-124">string</span><span class="sxs-lookup"><span data-stu-id="8acf2-124">string</span></span>  | <span data-ttu-id="8acf2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8acf2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8acf2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8acf2-127">Content-Type</span></span> | <span data-ttu-id="8acf2-128">string</span><span class="sxs-lookup"><span data-stu-id="8acf2-128">string</span></span>  | <span data-ttu-id="8acf2-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8acf2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8acf2-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8acf2-131">Request body</span></span>
<span data-ttu-id="8acf2-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8acf2-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8acf2-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="8acf2-133">Parameter</span></span>    | <span data-ttu-id="8acf2-134">Typ</span><span class="sxs-lookup"><span data-stu-id="8acf2-134">Type</span></span>   |<span data-ttu-id="8acf2-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8acf2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8acf2-136">comment</span><span class="sxs-lookup"><span data-stu-id="8acf2-136">comment</span></span>|<span data-ttu-id="8acf2-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8acf2-137">String</span></span>|<span data-ttu-id="8acf2-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="8acf2-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="8acf2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="8acf2-140">Response</span></span>

<span data-ttu-id="8acf2-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8acf2-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8acf2-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8acf2-143">Example</span></span>
<span data-ttu-id="8acf2-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8acf2-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8acf2-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8acf2-145">Request</span></span>
<span data-ttu-id="8acf2-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8acf2-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="8acf2-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8acf2-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8acf2-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="8acf2-148">Response</span></span>
<span data-ttu-id="8acf2-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8acf2-149">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
