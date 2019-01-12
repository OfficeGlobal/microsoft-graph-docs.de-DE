---
title: rejectedSender entfernen
description: Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „rejectedSenders“ entfernen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5b67968c805b36a93afc7841bfbe162abc2a89ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984542"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="c79b3-103">rejectedSender entfernen</span><span class="sxs-lookup"><span data-stu-id="c79b3-103">Remove rejectedSender</span></span>

> <span data-ttu-id="c79b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c79b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c79b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c79b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c79b3-106">Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „rejectedSenders“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="c79b3-106">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="c79b3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c79b3-107">Permissions</span></span>
<span data-ttu-id="c79b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c79b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c79b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c79b3-110">Permission type</span></span>                        | <span data-ttu-id="c79b3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c79b3-111">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="c79b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c79b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c79b3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c79b3-113">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="c79b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c79b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c79b3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79b3-115">Not supported.</span></span> |
| <span data-ttu-id="c79b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c79b3-116">Application</span></span>                            | <span data-ttu-id="c79b3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c79b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="c79b3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c79b3-119">Request headers</span></span>

| <span data-ttu-id="c79b3-120">Header</span><span class="sxs-lookup"><span data-stu-id="c79b3-120">Header</span></span>         | <span data-ttu-id="c79b3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c79b3-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c79b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c79b3-122">Authorization</span></span>  | <span data-ttu-id="c79b3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c79b3-p103">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="c79b3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c79b3-125">Request body</span></span>
<span data-ttu-id="c79b3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c79b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c79b3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79b3-127">Response</span></span>
<span data-ttu-id="c79b3-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c79b3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c79b3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c79b3-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c79b3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79b3-131">Request</span></span>
<span data-ttu-id="c79b3-132">Nachfolgend finden Sie ein paar Beispiele der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c79b3-132">The following are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="c79b3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79b3-133">Response</span></span>
<span data-ttu-id="c79b3-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c79b3-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
