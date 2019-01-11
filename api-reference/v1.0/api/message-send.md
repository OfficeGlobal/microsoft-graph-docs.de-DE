---
title: 'message: send'
description: Senden Sie eine Nachricht im Ordner "Entwürfe". Die Entwurf einer Nachricht kann eine neue Nachricht Entwurf, Antwort Entwurf, allen Antworten-Entwurfsdatenbank, oder
localization_priority: Priority
ms.openlocfilehash: cd98c4965f7eee3e53fc24bad551a1b14e8c7521
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867445"
---
# <a name="message-send"></a><span data-ttu-id="649b6-104">message: send</span><span class="sxs-lookup"><span data-stu-id="649b6-104">message: send</span></span>

<span data-ttu-id="649b6-p102">Sendet eine Nachricht im Ordner „Entwürfe“. Der Entwurf kann ein Entwurf für eine neue Nachricht, eine Antwort, eine Antwort an alle oder eine Weiterleitung sein. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.</span><span class="sxs-lookup"><span data-stu-id="649b6-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="649b6-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="649b6-108">Permissions</span></span>

<span data-ttu-id="649b6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="649b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="649b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="649b6-111">Permission type</span></span>      | <span data-ttu-id="649b6-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="649b6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="649b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="649b6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="649b6-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="649b6-114">Mail.Send</span></span>    |
|<span data-ttu-id="649b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="649b6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="649b6-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="649b6-116">Mail.Send</span></span>    |
|<span data-ttu-id="649b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="649b6-117">Application</span></span> | <span data-ttu-id="649b6-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="649b6-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="649b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="649b6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="649b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="649b6-120">Request headers</span></span>

| <span data-ttu-id="649b6-121">Name</span><span class="sxs-lookup"><span data-stu-id="649b6-121">Name</span></span>       | <span data-ttu-id="649b6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="649b6-122">Type</span></span> | <span data-ttu-id="649b6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="649b6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="649b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="649b6-124">Authorization</span></span>  | <span data-ttu-id="649b6-125">string</span><span class="sxs-lookup"><span data-stu-id="649b6-125">string</span></span>  | <span data-ttu-id="649b6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="649b6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="649b6-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="649b6-128">Content-Length</span></span> | <span data-ttu-id="649b6-129">number</span><span class="sxs-lookup"><span data-stu-id="649b6-129">number</span></span> | <span data-ttu-id="649b6-130">0. erforderlich.</span><span class="sxs-lookup"><span data-stu-id="649b6-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="649b6-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="649b6-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="649b6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="649b6-132">Response</span></span>

<span data-ttu-id="649b6-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="649b6-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="649b6-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="649b6-135">Example</span></span>

<span data-ttu-id="649b6-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="649b6-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="649b6-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="649b6-137">Request</span></span>

<span data-ttu-id="649b6-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="649b6-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="649b6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="649b6-139">Response</span></span>

<span data-ttu-id="649b6-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="649b6-140">Here is an example of the response.</span></span>
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
