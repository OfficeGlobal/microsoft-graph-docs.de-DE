---
title: 'group: subscribeByMail'
description: Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.
localization_priority: Normal
ms.openlocfilehash: 4127ae68caba0295426f81dc1c0c537ee2fb96b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837982"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="26aff-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="26aff-104">group: subscribeByMail</span></span>
<span data-ttu-id="26aff-p102">Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26aff-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="26aff-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="26aff-107">Permissions</span></span>
<span data-ttu-id="26aff-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26aff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26aff-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26aff-110">Permission type</span></span>      | <span data-ttu-id="26aff-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26aff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26aff-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26aff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26aff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26aff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26aff-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26aff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26aff-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26aff-115">Not supported.</span></span>    |
|<span data-ttu-id="26aff-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26aff-116">Application</span></span> | <span data-ttu-id="26aff-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26aff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26aff-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26aff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="26aff-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26aff-119">Request headers</span></span>
| <span data-ttu-id="26aff-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="26aff-120">Header</span></span>       | <span data-ttu-id="26aff-121">Wert</span><span class="sxs-lookup"><span data-stu-id="26aff-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26aff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26aff-122">Authorization</span></span>  | <span data-ttu-id="26aff-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="26aff-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26aff-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="26aff-125">Prefer</span></span> | <span data-ttu-id="26aff-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="26aff-126">return=minimal.</span></span> <span data-ttu-id="26aff-127">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="26aff-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="26aff-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="26aff-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="26aff-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26aff-129">Request body</span></span>
<span data-ttu-id="26aff-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="26aff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26aff-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="26aff-131">Response</span></span>
<span data-ttu-id="26aff-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26aff-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26aff-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26aff-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="26aff-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26aff-135">Request</span></span>
<span data-ttu-id="26aff-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26aff-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="26aff-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="26aff-137">Response</span></span>
<span data-ttu-id="26aff-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="26aff-138">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
