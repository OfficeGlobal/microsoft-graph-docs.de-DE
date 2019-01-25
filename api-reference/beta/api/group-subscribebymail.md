---
title: 'group: subscribeByMail'
description: Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0a334daa005947099da324aab31ccc2a1da6b6e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516420"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="16dda-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="16dda-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16dda-105">Durch Aufrufen dieser Methode wird den aktuellen Benutzer zum Empfangen von e-Mail-Benachrichtigungen für diese Gruppe, zu der neuen Beiträge, Ereignisse und Dateien in dieser Gruppe aktivieren.</span><span class="sxs-lookup"><span data-stu-id="16dda-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="16dda-106">Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16dda-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="16dda-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="16dda-107">Permissions</span></span>
<span data-ttu-id="16dda-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16dda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16dda-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16dda-110">Permission type</span></span>      | <span data-ttu-id="16dda-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16dda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16dda-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16dda-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16dda-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dda-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16dda-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16dda-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16dda-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16dda-115">Not supported.</span></span>    |
|<span data-ttu-id="16dda-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16dda-116">Application</span></span> | <span data-ttu-id="16dda-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16dda-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16dda-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16dda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="16dda-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16dda-119">Request headers</span></span>
| <span data-ttu-id="16dda-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="16dda-120">Header</span></span>       | <span data-ttu-id="16dda-121">Wert</span><span class="sxs-lookup"><span data-stu-id="16dda-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16dda-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16dda-122">Authorization</span></span>  | <span data-ttu-id="16dda-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16dda-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16dda-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="16dda-125">Prefer</span></span> | <span data-ttu-id="16dda-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="16dda-126">return=minimal.</span></span> <span data-ttu-id="16dda-127">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="16dda-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="16dda-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="16dda-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="16dda-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="16dda-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="16dda-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="16dda-130">Response</span></span>
<span data-ttu-id="16dda-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16dda-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16dda-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16dda-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16dda-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16dda-134">Request</span></span>
<span data-ttu-id="16dda-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16dda-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="16dda-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="16dda-136">Response</span></span>
<span data-ttu-id="16dda-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="16dda-137">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
