---
title: 'group: resetUnseenCount'
description: Zurücksetzen der UnseenCount der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde. Unterstützt nur die Office 365-Gruppen.
ms.openlocfilehash: b6218176f097759870aad4a3a2908759862002e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065422"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="01c61-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="01c61-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="01c61-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01c61-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01c61-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01c61-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01c61-107">Zurücksetzen der UnseenCount der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde.</span><span class="sxs-lookup"><span data-stu-id="01c61-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="01c61-108">Unterstützt nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="01c61-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="01c61-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="01c61-109">Permissions</span></span>
<span data-ttu-id="01c61-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01c61-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01c61-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01c61-112">Permission type</span></span>      | <span data-ttu-id="01c61-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01c61-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01c61-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01c61-114">Delegated (work or school account)</span></span> | <span data-ttu-id="01c61-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01c61-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01c61-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01c61-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01c61-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01c61-117">Not supported.</span></span>    |
|<span data-ttu-id="01c61-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01c61-118">Application</span></span> | <span data-ttu-id="01c61-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01c61-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01c61-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01c61-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="01c61-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01c61-121">Request headers</span></span>
| <span data-ttu-id="01c61-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="01c61-122">Header</span></span>       | <span data-ttu-id="01c61-123">Wert</span><span class="sxs-lookup"><span data-stu-id="01c61-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01c61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="01c61-124">Authorization</span></span>  | <span data-ttu-id="01c61-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01c61-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01c61-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="01c61-127">Prefer</span></span> | <span data-ttu-id="01c61-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="01c61-128">return=minimal.</span></span> <span data-ttu-id="01c61-129">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="01c61-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="01c61-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="01c61-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="01c61-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01c61-131">Request body</span></span>
<span data-ttu-id="01c61-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="01c61-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01c61-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="01c61-133">Response</span></span>
<span data-ttu-id="01c61-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01c61-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01c61-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01c61-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01c61-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01c61-137">Request</span></span>
<span data-ttu-id="01c61-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01c61-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="01c61-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="01c61-139">Response</span></span>
<span data-ttu-id="01c61-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="01c61-140">The following is an example of the response.</span></span> 
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
