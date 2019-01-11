---
title: 'group: subscribeByMail'
description: Durch Aufrufen dieser Methode wird den aktuellen Benutzer zum Empfangen von e-Mail-Benachrichtigungen für diese Gruppe, zu der neuen Beiträge, Ereignisse und Dateien in dieser Gruppe aktivieren. Unterstützt nur die Office 365-Gruppen.
localization_priority: Normal
ms.openlocfilehash: 5cbb5d461f5e3cc71790f6546c6ebf638ffa31d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813167"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="9bd3b-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="9bd3b-104">group: subscribeByMail</span></span>

> <span data-ttu-id="9bd3b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bd3b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bd3b-107">Durch Aufrufen dieser Methode wird den aktuellen Benutzer zum Empfangen von e-Mail-Benachrichtigungen für diese Gruppe, zu der neuen Beiträge, Ereignisse und Dateien in dieser Gruppe aktivieren.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-107">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="9bd3b-108">Unterstützt nur die Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bd3b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9bd3b-109">Permissions</span></span>
<span data-ttu-id="9bd3b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bd3b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd3b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bd3b-112">Permission type</span></span>      | <span data-ttu-id="9bd3b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bd3b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd3b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bd3b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd3b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd3b-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9bd3b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bd3b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd3b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bd3b-117">Not supported.</span></span>    |
|<span data-ttu-id="9bd3b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bd3b-118">Application</span></span> | <span data-ttu-id="9bd3b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bd3b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bd3b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bd3b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="9bd3b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bd3b-121">Request headers</span></span>
| <span data-ttu-id="9bd3b-122">Header</span><span class="sxs-lookup"><span data-stu-id="9bd3b-122">Header</span></span>       | <span data-ttu-id="9bd3b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9bd3b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bd3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd3b-124">Authorization</span></span>  | <span data-ttu-id="9bd3b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9bd3b-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="9bd3b-127">Prefer</span></span> | <span data-ttu-id="9bd3b-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-128">return=minimal.</span></span> <span data-ttu-id="9bd3b-129">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="9bd3b-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="9bd3b-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="9bd3b-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bd3b-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9bd3b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bd3b-132">Response</span></span>
<span data-ttu-id="9bd3b-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bd3b-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bd3b-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9bd3b-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bd3b-136">Request</span></span>
<span data-ttu-id="9bd3b-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="9bd3b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bd3b-138">Response</span></span>
<span data-ttu-id="9bd3b-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9bd3b-139">The following is an example of the response.</span></span> 
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
