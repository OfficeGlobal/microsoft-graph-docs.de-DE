---
title: 'Rufen Sie: ChangeScreenSharingRole'
description: Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf. Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f0bdd9a4c8e900d9a1ec5f7801fa959ebdaae1e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514733"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="50c69-104">Rufen Sie: ChangeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="50c69-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50c69-105">Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="50c69-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="50c69-106">Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="50c69-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="50c69-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50c69-107">Permissions</span></span>
<span data-ttu-id="50c69-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50c69-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50c69-110">Permission type</span></span>                        | <span data-ttu-id="50c69-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50c69-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50c69-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50c69-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="50c69-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50c69-113">Not Supported</span></span>                               |
| <span data-ttu-id="50c69-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50c69-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50c69-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50c69-115">Not Supported</span></span>                               |
| <span data-ttu-id="50c69-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50c69-116">Application</span></span>                            | <span data-ttu-id="50c69-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="50c69-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="50c69-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50c69-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="50c69-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50c69-119">Request headers</span></span>
| <span data-ttu-id="50c69-120">Name</span><span class="sxs-lookup"><span data-stu-id="50c69-120">Name</span></span>          | <span data-ttu-id="50c69-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50c69-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="50c69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c69-122">Authorization</span></span> | <span data-ttu-id="50c69-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50c69-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50c69-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50c69-125">Request body</span></span>
<span data-ttu-id="50c69-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="50c69-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50c69-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="50c69-127">Parameter</span></span>      | <span data-ttu-id="50c69-128">Typ</span><span class="sxs-lookup"><span data-stu-id="50c69-128">Type</span></span>    |<span data-ttu-id="50c69-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50c69-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50c69-130">role</span><span class="sxs-lookup"><span data-stu-id="50c69-130">role</span></span>|<span data-ttu-id="50c69-131">String</span><span class="sxs-lookup"><span data-stu-id="50c69-131">String</span></span>|<span data-ttu-id="50c69-132">Mögliche Werte sind: 'Viewer', 'Mitbenutzenden'</span><span class="sxs-lookup"><span data-stu-id="50c69-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="50c69-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="50c69-133">Response</span></span>
<span data-ttu-id="50c69-134">Gibt `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="50c69-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50c69-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50c69-135">Example</span></span>
<span data-ttu-id="50c69-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="50c69-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50c69-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50c69-137">Request</span></span>
<span data-ttu-id="50c69-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="50c69-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="50c69-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="50c69-139">Response</span></span>
<span data-ttu-id="50c69-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50c69-140">Here is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
