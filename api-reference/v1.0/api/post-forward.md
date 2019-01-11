---
title: 'post: forward'
description: 'Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können die übergeordnete Unterhaltung und die Thread in der Anforderung angeben, '
localization_priority: Normal
ms.openlocfilehash: b670338061d70b4ee8663d443d1bb5706f9e9157
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837324"
---
# <a name="post-forward"></a><span data-ttu-id="1aca5-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="1aca5-104">post: forward</span></span>

<span data-ttu-id="1aca5-p102">Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="1aca5-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1aca5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1aca5-107">Permissions</span></span>
<span data-ttu-id="1aca5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aca5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aca5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1aca5-110">Permission type</span></span>      | <span data-ttu-id="1aca5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1aca5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aca5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1aca5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1aca5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aca5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1aca5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1aca5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aca5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1aca5-115">Not supported.</span></span>    |
|<span data-ttu-id="1aca5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1aca5-116">Application</span></span> | <span data-ttu-id="1aca5-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aca5-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aca5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1aca5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="1aca5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1aca5-119">Request headers</span></span>
| <span data-ttu-id="1aca5-120">Header</span><span class="sxs-lookup"><span data-stu-id="1aca5-120">Header</span></span>       | <span data-ttu-id="1aca5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1aca5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1aca5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aca5-122">Authorization</span></span>  | <span data-ttu-id="1aca5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1aca5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1aca5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1aca5-125">Request body</span></span>
<span data-ttu-id="1aca5-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1aca5-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1aca5-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="1aca5-127">Parameter</span></span>    | <span data-ttu-id="1aca5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1aca5-128">Type</span></span>   |<span data-ttu-id="1aca5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1aca5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aca5-130">comment</span><span class="sxs-lookup"><span data-stu-id="1aca5-130">comment</span></span>|<span data-ttu-id="1aca5-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1aca5-131">String</span></span>|<span data-ttu-id="1aca5-132">Optionaler Kommentar, der zusammen mit dem Beitrag weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="1aca5-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="1aca5-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="1aca5-133">toRecipients</span></span>|<span data-ttu-id="1aca5-134">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1aca5-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="1aca5-135">Die Empfänger, an die der Thread weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="1aca5-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="1aca5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1aca5-136">Response</span></span>

<span data-ttu-id="1aca5-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1aca5-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aca5-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1aca5-139">Example</span></span>
<span data-ttu-id="1aca5-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1aca5-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1aca5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1aca5-141">Request</span></span>
<span data-ttu-id="1aca5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1aca5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="1aca5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1aca5-143">Response</span></span>
<span data-ttu-id="1aca5-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1aca5-144">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
