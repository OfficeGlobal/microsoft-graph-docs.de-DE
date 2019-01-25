---
title: 'group: resetUnseenCount'
description: Dient zum Zurücksetzen des unseenCount-Elements aller Beiträge, die der aktuelle Benutzer seit dem letzten Besuch noch nicht gesehen hat. Wird nur für Office 365-Gruppen unterstützt.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: aa37261a536437d0e82195ecfaae06de9e1c6a3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524814"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="2532f-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="2532f-104">group: resetUnseenCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2532f-105">Zurücksetzen der UnseenCount der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde.</span><span class="sxs-lookup"><span data-stu-id="2532f-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="2532f-106">Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2532f-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="2532f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2532f-107">Permissions</span></span>
<span data-ttu-id="2532f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2532f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2532f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2532f-110">Permission type</span></span>      | <span data-ttu-id="2532f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2532f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2532f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2532f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2532f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2532f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2532f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2532f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2532f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2532f-115">Not supported.</span></span>    |
|<span data-ttu-id="2532f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2532f-116">Application</span></span> | <span data-ttu-id="2532f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2532f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2532f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2532f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="2532f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2532f-119">Request headers</span></span>
| <span data-ttu-id="2532f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2532f-120">Header</span></span>       | <span data-ttu-id="2532f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2532f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2532f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2532f-122">Authorization</span></span>  | <span data-ttu-id="2532f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2532f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2532f-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="2532f-125">Prefer</span></span> | <span data-ttu-id="2532f-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="2532f-126">return=minimal.</span></span> <span data-ttu-id="2532f-127">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="2532f-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="2532f-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="2532f-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2532f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2532f-129">Request body</span></span>
<span data-ttu-id="2532f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2532f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2532f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2532f-131">Response</span></span>
<span data-ttu-id="2532f-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2532f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2532f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2532f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2532f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2532f-135">Request</span></span>
<span data-ttu-id="2532f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2532f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="2532f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2532f-137">Response</span></span>
<span data-ttu-id="2532f-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2532f-138">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-resetunseencount.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
