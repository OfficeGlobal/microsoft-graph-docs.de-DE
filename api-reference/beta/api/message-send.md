---
title: 'message: send'
description: Senden Sie eine Nachricht im Ordner "Entwürfe". Die Entwurf einer Nachricht kann eine neue Nachricht Entwurf, Antwort Entwurf, allen Antworten-Entwurfsdatenbank, oder
localization_priority: Normal
ms.openlocfilehash: 6ccef4d1a58faea7678acefee5d175403a8827b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806643"
---
# <a name="message-send"></a><span data-ttu-id="918f3-104">message: send</span><span class="sxs-lookup"><span data-stu-id="918f3-104">message: send</span></span>

> <span data-ttu-id="918f3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="918f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="918f3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="918f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="918f3-p103">Sendet eine Nachricht im Ordner „Entwürfe“. Der Entwurf kann ein Entwurf für eine neue Nachricht, eine Antwort, eine Antwort an alle oder eine Weiterleitung sein. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="918f3-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="918f3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="918f3-110">Permissions</span></span>

<span data-ttu-id="918f3-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="918f3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="918f3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="918f3-113">Permission type</span></span>      | <span data-ttu-id="918f3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="918f3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="918f3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="918f3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="918f3-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="918f3-116">Mail.Send</span></span>    |
|<span data-ttu-id="918f3-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="918f3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="918f3-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="918f3-118">Mail.Send</span></span>    |
|<span data-ttu-id="918f3-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="918f3-119">Application</span></span> | <span data-ttu-id="918f3-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="918f3-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="918f3-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="918f3-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="918f3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="918f3-122">Request headers</span></span>

| <span data-ttu-id="918f3-123">Name</span><span class="sxs-lookup"><span data-stu-id="918f3-123">Name</span></span>       | <span data-ttu-id="918f3-124">Typ</span><span class="sxs-lookup"><span data-stu-id="918f3-124">Type</span></span> | <span data-ttu-id="918f3-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="918f3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="918f3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="918f3-126">Authorization</span></span>  | <span data-ttu-id="918f3-127">string</span><span class="sxs-lookup"><span data-stu-id="918f3-127">string</span></span>  | <span data-ttu-id="918f3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="918f3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="918f3-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="918f3-130">Content-Length</span></span> | <span data-ttu-id="918f3-131">number</span><span class="sxs-lookup"><span data-stu-id="918f3-131">number</span></span> | <span data-ttu-id="918f3-132">0. erforderlich.</span><span class="sxs-lookup"><span data-stu-id="918f3-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="918f3-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="918f3-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="918f3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="918f3-134">Response</span></span>

<span data-ttu-id="918f3-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="918f3-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="918f3-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="918f3-137">Example</span></span>

<span data-ttu-id="918f3-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="918f3-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="918f3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="918f3-139">Request</span></span>

<span data-ttu-id="918f3-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="918f3-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="918f3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="918f3-141">Response</span></span>

<span data-ttu-id="918f3-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="918f3-142">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
