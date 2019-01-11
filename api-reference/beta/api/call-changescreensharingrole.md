---
title: 'Rufen Sie: ChangeScreenSharingRole'
description: Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf. Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 64c85025a7aa1f3095fe6ddd8d7d398348a2a1ce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865009"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="f9ae6-104">Rufen Sie: ChangeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="f9ae6-104">call: changeScreenSharingRole</span></span>

> <span data-ttu-id="f9ae6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9ae6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9ae6-107">Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-107">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="f9ae6-108">Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-108">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9ae6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9ae6-109">Permissions</span></span>
<span data-ttu-id="f9ae6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ae6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9ae6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9ae6-112">Permission type</span></span>                        | <span data-ttu-id="f9ae6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9ae6-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9ae6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9ae6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9ae6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9ae6-115">Not Supported</span></span>                               |
| <span data-ttu-id="f9ae6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9ae6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ae6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9ae6-117">Not Supported</span></span>                               |
| <span data-ttu-id="f9ae6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9ae6-118">Application</span></span>                            | <span data-ttu-id="f9ae6-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f9ae6-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f9ae6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9ae6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="f9ae6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9ae6-121">Request headers</span></span>
| <span data-ttu-id="f9ae6-122">Name</span><span class="sxs-lookup"><span data-stu-id="f9ae6-122">Name</span></span>          | <span data-ttu-id="f9ae6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ae6-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f9ae6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ae6-124">Authorization</span></span> | <span data-ttu-id="f9ae6-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ae6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9ae6-127">Request body</span></span>
<span data-ttu-id="f9ae6-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9ae6-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="f9ae6-129">Parameter</span></span>      | <span data-ttu-id="f9ae6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f9ae6-130">Type</span></span>    |<span data-ttu-id="f9ae6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ae6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9ae6-132">role</span><span class="sxs-lookup"><span data-stu-id="f9ae6-132">role</span></span>|<span data-ttu-id="f9ae6-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9ae6-133">String</span></span>|<span data-ttu-id="f9ae6-134">Mögliche Werte sind: 'Viewer', 'Mitbenutzenden'</span><span class="sxs-lookup"><span data-stu-id="f9ae6-134">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="f9ae6-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9ae6-135">Response</span></span>
<span data-ttu-id="f9ae6-136">Gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-136">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9ae6-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9ae6-137">Example</span></span>
<span data-ttu-id="f9ae6-138">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f9ae6-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9ae6-139">Request</span></span>
<span data-ttu-id="f9ae6-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="f9ae6-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9ae6-141">Response</span></span>
<span data-ttu-id="f9ae6-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9ae6-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
