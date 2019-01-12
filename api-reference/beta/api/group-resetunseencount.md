---
title: 'group: resetUnseenCount'
description: Zurücksetzen der UnseenCount der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde. Unterstützt nur die Office 365-Gruppen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3d85dc82efd67311b81d69f2f99e63c47155f15a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926281"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="738cb-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="738cb-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="738cb-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="738cb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="738cb-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="738cb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="738cb-107">Zurücksetzen der UnseenCount der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde.</span><span class="sxs-lookup"><span data-stu-id="738cb-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="738cb-108">Unterstützt nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="738cb-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="738cb-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="738cb-109">Permissions</span></span>
<span data-ttu-id="738cb-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="738cb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="738cb-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="738cb-112">Permission type</span></span>      | <span data-ttu-id="738cb-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="738cb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="738cb-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="738cb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="738cb-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="738cb-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="738cb-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="738cb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="738cb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="738cb-117">Not supported.</span></span>    |
|<span data-ttu-id="738cb-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="738cb-118">Application</span></span> | <span data-ttu-id="738cb-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="738cb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="738cb-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="738cb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="738cb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="738cb-121">Request headers</span></span>
| <span data-ttu-id="738cb-122">Header</span><span class="sxs-lookup"><span data-stu-id="738cb-122">Header</span></span>       | <span data-ttu-id="738cb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="738cb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="738cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="738cb-124">Authorization</span></span>  | <span data-ttu-id="738cb-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="738cb-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="738cb-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="738cb-127">Prefer</span></span> | <span data-ttu-id="738cb-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="738cb-128">return=minimal.</span></span> <span data-ttu-id="738cb-129">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="738cb-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="738cb-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="738cb-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="738cb-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="738cb-131">Request body</span></span>
<span data-ttu-id="738cb-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="738cb-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="738cb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="738cb-133">Response</span></span>
<span data-ttu-id="738cb-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="738cb-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="738cb-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="738cb-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="738cb-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="738cb-137">Request</span></span>
<span data-ttu-id="738cb-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="738cb-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="738cb-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="738cb-139">Response</span></span>
<span data-ttu-id="738cb-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="738cb-140">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
