---
title: 'message: replyAll'
description: Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8e2d9b2481e4fb0fc4e6e166dae1189baa77b7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884308"
---
# <a name="message-replyall"></a><span data-ttu-id="85c77-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="85c77-104">message: replyAll</span></span>

<span data-ttu-id="85c77-p102">Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="85c77-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="85c77-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85c77-107">Permissions</span></span>
<span data-ttu-id="85c77-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c77-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c77-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85c77-110">Permission type</span></span>      | <span data-ttu-id="85c77-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85c77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c77-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85c77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85c77-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85c77-113">Mail.Send</span></span>    |
|<span data-ttu-id="85c77-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85c77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c77-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85c77-115">Mail.Send</span></span>    |
|<span data-ttu-id="85c77-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85c77-116">Application</span></span> | <span data-ttu-id="85c77-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85c77-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="85c77-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85c77-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="85c77-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85c77-119">Request headers</span></span>
| <span data-ttu-id="85c77-120">Name</span><span class="sxs-lookup"><span data-stu-id="85c77-120">Name</span></span>       | <span data-ttu-id="85c77-121">Typ</span><span class="sxs-lookup"><span data-stu-id="85c77-121">Type</span></span> | <span data-ttu-id="85c77-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85c77-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85c77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c77-123">Authorization</span></span>  | <span data-ttu-id="85c77-124">string</span><span class="sxs-lookup"><span data-stu-id="85c77-124">string</span></span>  | <span data-ttu-id="85c77-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85c77-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85c77-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85c77-127">Content-Type</span></span> | <span data-ttu-id="85c77-128">string</span><span class="sxs-lookup"><span data-stu-id="85c77-128">string</span></span>  | <span data-ttu-id="85c77-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85c77-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85c77-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85c77-131">Request body</span></span>
<span data-ttu-id="85c77-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="85c77-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85c77-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="85c77-133">Parameter</span></span>    | <span data-ttu-id="85c77-134">Typ</span><span class="sxs-lookup"><span data-stu-id="85c77-134">Type</span></span>   |<span data-ttu-id="85c77-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85c77-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85c77-136">comment</span><span class="sxs-lookup"><span data-stu-id="85c77-136">comment</span></span>|<span data-ttu-id="85c77-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85c77-137">String</span></span>|<span data-ttu-id="85c77-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="85c77-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="85c77-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="85c77-140">Response</span></span>

<span data-ttu-id="85c77-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85c77-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c77-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85c77-143">Example</span></span>
<span data-ttu-id="85c77-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="85c77-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85c77-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85c77-145">Request</span></span>
<span data-ttu-id="85c77-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85c77-146">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="85c77-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="85c77-147">Response</span></span>
<span data-ttu-id="85c77-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="85c77-148">Here is an example of the response.</span></span>
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
