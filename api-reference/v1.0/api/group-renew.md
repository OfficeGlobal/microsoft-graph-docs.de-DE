---
title: 'group: renew'
description: Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 46a51d0a1d4bea5cebc4c3178f6776d80f313fbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922732"
---
# <a name="group-renew"></a><span data-ttu-id="c92c1-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="c92c1-104">group: renew</span></span>

<span data-ttu-id="c92c1-105">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c92c1-105">Renews a group's expiration.</span></span> <span data-ttu-id="c92c1-106">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="c92c1-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c92c1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c92c1-107">Permissions</span></span>

<span data-ttu-id="c92c1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c92c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c92c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c92c1-110">Permission type</span></span>      | <span data-ttu-id="c92c1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c92c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c92c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c92c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c92c1-113">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c92c1-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c92c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c92c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c92c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c92c1-115">Not supported</span></span> |
|<span data-ttu-id="c92c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c92c1-116">Application</span></span> | <span data-ttu-id="c92c1-117">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c92c1-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c92c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c92c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="c92c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c92c1-119">Request headers</span></span>
| <span data-ttu-id="c92c1-120">Name</span><span class="sxs-lookup"><span data-stu-id="c92c1-120">Name</span></span>       | <span data-ttu-id="c92c1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c92c1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c92c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c92c1-122">Authorization</span></span>  | <span data-ttu-id="c92c1-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c92c1-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="c92c1-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c92c1-124">Request body</span></span>

<span data-ttu-id="c92c1-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c92c1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c92c1-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="c92c1-126">Response</span></span>

<span data-ttu-id="c92c1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c92c1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c92c1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c92c1-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c92c1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c92c1-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="c92c1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c92c1-131">Response</span></span>
<span data-ttu-id="c92c1-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c92c1-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
