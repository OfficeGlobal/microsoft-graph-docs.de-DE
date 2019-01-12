---
title: 'message: send'
description: Senden Sie eine Nachricht im Ordner "Entwürfe". Die Entwurf einer Nachricht kann eine neue Nachricht Entwurf, Antwort Entwurf, allen Antworten-Entwurfsdatenbank, oder
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 937c2da1bab83c412097f4207f32d07dc98d2ff8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940673"
---
# <a name="message-send"></a><span data-ttu-id="48bce-104">message: send</span><span class="sxs-lookup"><span data-stu-id="48bce-104">message: send</span></span>

> <span data-ttu-id="48bce-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48bce-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48bce-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48bce-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48bce-p103">Sendet eine Nachricht im Ordner „Entwürfe“. Der Entwurf kann ein Entwurf für eine neue Nachricht, eine Antwort, eine Antwort an alle oder eine Weiterleitung sein. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="48bce-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="48bce-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48bce-110">Permissions</span></span>

<span data-ttu-id="48bce-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48bce-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48bce-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48bce-113">Permission type</span></span>      | <span data-ttu-id="48bce-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48bce-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48bce-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48bce-115">Delegated (work or school account)</span></span> | <span data-ttu-id="48bce-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48bce-116">Mail.Send</span></span>    |
|<span data-ttu-id="48bce-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48bce-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48bce-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48bce-118">Mail.Send</span></span>    |
|<span data-ttu-id="48bce-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48bce-119">Application</span></span> | <span data-ttu-id="48bce-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="48bce-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="48bce-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48bce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="48bce-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48bce-122">Request headers</span></span>

| <span data-ttu-id="48bce-123">Name</span><span class="sxs-lookup"><span data-stu-id="48bce-123">Name</span></span>       | <span data-ttu-id="48bce-124">Typ</span><span class="sxs-lookup"><span data-stu-id="48bce-124">Type</span></span> | <span data-ttu-id="48bce-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48bce-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48bce-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="48bce-126">Authorization</span></span>  | <span data-ttu-id="48bce-127">string</span><span class="sxs-lookup"><span data-stu-id="48bce-127">string</span></span>  | <span data-ttu-id="48bce-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48bce-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48bce-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="48bce-130">Content-Length</span></span> | <span data-ttu-id="48bce-131">number</span><span class="sxs-lookup"><span data-stu-id="48bce-131">number</span></span> | <span data-ttu-id="48bce-132">0. erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48bce-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48bce-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48bce-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="48bce-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="48bce-134">Response</span></span>

<span data-ttu-id="48bce-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48bce-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48bce-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48bce-137">Example</span></span>

<span data-ttu-id="48bce-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="48bce-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48bce-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48bce-139">Request</span></span>

<span data-ttu-id="48bce-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48bce-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="48bce-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="48bce-141">Response</span></span>

<span data-ttu-id="48bce-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48bce-142">Here is an example of the response.</span></span>
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
