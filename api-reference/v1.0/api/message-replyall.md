---
title: 'message: replyAll'
description: Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.
author: angelgolfer-ms
ms.openlocfilehash: cefe4d92d23cb9531f6fa66f74d1c9af87ef429e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348986"
---
# <a name="message-replyall"></a><span data-ttu-id="547de-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="547de-104">message: replyAll</span></span>

<span data-ttu-id="547de-p102">Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="547de-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="547de-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="547de-107">Permissions</span></span>
<span data-ttu-id="547de-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="547de-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="547de-110">Permission type</span></span>      | <span data-ttu-id="547de-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="547de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="547de-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="547de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="547de-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="547de-113">Mail.Send</span></span>    |
|<span data-ttu-id="547de-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="547de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547de-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="547de-115">Mail.Send</span></span>    |
|<span data-ttu-id="547de-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="547de-116">Application</span></span> | <span data-ttu-id="547de-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="547de-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="547de-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="547de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="547de-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="547de-119">Request headers</span></span>
| <span data-ttu-id="547de-120">Name</span><span class="sxs-lookup"><span data-stu-id="547de-120">Name</span></span>       | <span data-ttu-id="547de-121">Typ</span><span class="sxs-lookup"><span data-stu-id="547de-121">Type</span></span> | <span data-ttu-id="547de-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="547de-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="547de-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="547de-123">Authorization</span></span>  | <span data-ttu-id="547de-124">string</span><span class="sxs-lookup"><span data-stu-id="547de-124">string</span></span>  | <span data-ttu-id="547de-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="547de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="547de-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="547de-127">Content-Type</span></span> | <span data-ttu-id="547de-128">string</span><span class="sxs-lookup"><span data-stu-id="547de-128">string</span></span>  | <span data-ttu-id="547de-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="547de-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="547de-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="547de-131">Request body</span></span>
<span data-ttu-id="547de-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="547de-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="547de-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="547de-133">Parameter</span></span>    | <span data-ttu-id="547de-134">Typ</span><span class="sxs-lookup"><span data-stu-id="547de-134">Type</span></span>   |<span data-ttu-id="547de-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="547de-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="547de-136">comment</span><span class="sxs-lookup"><span data-stu-id="547de-136">comment</span></span>|<span data-ttu-id="547de-137">String</span><span class="sxs-lookup"><span data-stu-id="547de-137">String</span></span>|<span data-ttu-id="547de-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="547de-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="547de-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="547de-140">Response</span></span>

<span data-ttu-id="547de-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="547de-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="547de-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="547de-143">Example</span></span>
<span data-ttu-id="547de-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="547de-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="547de-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="547de-145">Request</span></span>
<span data-ttu-id="547de-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="547de-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="547de-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="547de-147">Response</span></span>
<span data-ttu-id="547de-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="547de-148">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
