---
title: 'post: forward'
description: 'Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können die übergeordnete Unterhaltung und die Thread in der Anforderung angeben, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 557eaa7455600fe6da864a70457b4f3094df8c41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512052"
---
# <a name="post-forward"></a><span data-ttu-id="d750a-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="d750a-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d750a-p102">Dient zum Weiterleiten eines Beitrags an einen Empfänger. Sie können sowohl die übergeordnete Unterhaltung als auch den Thread in der Anforderung angeben, oder Sie können nur den übergeordneten Thread ohne die übergeordnete Unterhaltung angeben.</span><span class="sxs-lookup"><span data-stu-id="d750a-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d750a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d750a-107">Permissions</span></span>
<span data-ttu-id="d750a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d750a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d750a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d750a-110">Permission type</span></span>      | <span data-ttu-id="d750a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d750a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d750a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d750a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d750a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d750a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d750a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d750a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d750a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d750a-115">Not supported.</span></span>    |
|<span data-ttu-id="d750a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d750a-116">Application</span></span> | <span data-ttu-id="d750a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d750a-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d750a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d750a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="d750a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d750a-119">Request headers</span></span>
| <span data-ttu-id="d750a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d750a-120">Header</span></span>       | <span data-ttu-id="d750a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d750a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d750a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d750a-122">Authorization</span></span>  | <span data-ttu-id="d750a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d750a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d750a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d750a-125">Request body</span></span>
<span data-ttu-id="d750a-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d750a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d750a-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="d750a-127">Parameter</span></span>    | <span data-ttu-id="d750a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="d750a-128">Type</span></span>   |<span data-ttu-id="d750a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d750a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d750a-130">comment</span><span class="sxs-lookup"><span data-stu-id="d750a-130">comment</span></span>|<span data-ttu-id="d750a-131">String</span><span class="sxs-lookup"><span data-stu-id="d750a-131">String</span></span>|<span data-ttu-id="d750a-132">Optionaler Kommentar, der zusammen mit dem Beitrag weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="d750a-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="d750a-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d750a-133">toRecipients</span></span>|<span data-ttu-id="d750a-134">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="d750a-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="d750a-135">Die Empfänger, an die der Thread weitergeleitet wird.</span><span class="sxs-lookup"><span data-stu-id="d750a-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="d750a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d750a-136">Response</span></span>

<span data-ttu-id="d750a-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d750a-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d750a-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d750a-139">Example</span></span>
<span data-ttu-id="d750a-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d750a-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d750a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d750a-141">Request</span></span>
<span data-ttu-id="d750a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d750a-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d750a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="d750a-143">Response</span></span>
<span data-ttu-id="d750a-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d750a-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
