---
title: 'post: forward'
description: 'Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können die übergeordnete Unterhaltung und die Thread in der Anforderung angeben, '
localization_priority: Normal
ms.openlocfilehash: 64b7d87745cf897ea827d37a9cd4f4c60d197068
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889439"
---
# <a name="post-forward"></a><span data-ttu-id="77e26-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="77e26-104">post: forward</span></span>

> <span data-ttu-id="77e26-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77e26-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77e26-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77e26-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77e26-p103">Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="77e26-p103">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="77e26-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77e26-109">Permissions</span></span>
<span data-ttu-id="77e26-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77e26-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e26-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77e26-112">Permission type</span></span>      | <span data-ttu-id="77e26-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77e26-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77e26-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77e26-114">Delegated (work or school account)</span></span> | <span data-ttu-id="77e26-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e26-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="77e26-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77e26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e26-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77e26-117">Not supported.</span></span>    |
|<span data-ttu-id="77e26-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77e26-118">Application</span></span> | <span data-ttu-id="77e26-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e26-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77e26-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77e26-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="77e26-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77e26-121">Request headers</span></span>
| <span data-ttu-id="77e26-122">Header</span><span class="sxs-lookup"><span data-stu-id="77e26-122">Header</span></span>       | <span data-ttu-id="77e26-123">Wert</span><span class="sxs-lookup"><span data-stu-id="77e26-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77e26-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e26-124">Authorization</span></span>  | <span data-ttu-id="77e26-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77e26-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77e26-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77e26-127">Request body</span></span>
<span data-ttu-id="77e26-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="77e26-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77e26-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="77e26-129">Parameter</span></span>    | <span data-ttu-id="77e26-130">Typ</span><span class="sxs-lookup"><span data-stu-id="77e26-130">Type</span></span>   |<span data-ttu-id="77e26-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77e26-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77e26-132">comment</span><span class="sxs-lookup"><span data-stu-id="77e26-132">comment</span></span>|<span data-ttu-id="77e26-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77e26-133">String</span></span>|<span data-ttu-id="77e26-134">Optionaler Kommentar, der zusammen mit dem Beitrag weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="77e26-134">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="77e26-135">toRecipients</span><span class="sxs-lookup"><span data-stu-id="77e26-135">toRecipients</span></span>|<span data-ttu-id="77e26-136">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="77e26-136">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="77e26-137">Die Empfänger, an die der Thread weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="77e26-137">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="77e26-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="77e26-138">Response</span></span>

<span data-ttu-id="77e26-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77e26-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77e26-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77e26-141">Example</span></span>
<span data-ttu-id="77e26-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="77e26-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="77e26-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77e26-143">Request</span></span>
<span data-ttu-id="77e26-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77e26-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="77e26-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="77e26-145">Response</span></span>
<span data-ttu-id="77e26-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="77e26-146">Here is an example of the response.</span></span>
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
