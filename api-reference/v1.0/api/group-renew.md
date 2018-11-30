---
title: 'group: renew'
description: Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.
ms.openlocfilehash: 82cbc4f982b5636cc53436091a40492d7ad83afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017959"
---
# <a name="group-renew"></a><span data-ttu-id="3dff5-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="3dff5-104">group: renew</span></span>

<span data-ttu-id="3dff5-105">Verlängert den Ablaufzeitraum einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="3dff5-105">Renews a group's expiration.</span></span> <span data-ttu-id="3dff5-106">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="3dff5-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dff5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3dff5-107">Permissions</span></span>

<span data-ttu-id="3dff5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dff5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="3dff5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3dff5-110">Permission type</span></span>      | <span data-ttu-id="3dff5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3dff5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dff5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3dff5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3dff5-113">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dff5-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dff5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3dff5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dff5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3dff5-115">Not supported</span></span> |
|<span data-ttu-id="3dff5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3dff5-116">Application</span></span> | <span data-ttu-id="3dff5-117">Group.ReadWrite.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dff5-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dff5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3dff5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="3dff5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3dff5-119">Request headers</span></span>
| <span data-ttu-id="3dff5-120">Name</span><span class="sxs-lookup"><span data-stu-id="3dff5-120">Name</span></span>       | <span data-ttu-id="3dff5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3dff5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3dff5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dff5-122">Authorization</span></span>  | <span data-ttu-id="3dff5-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3dff5-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="3dff5-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3dff5-124">Request body</span></span>

<span data-ttu-id="3dff5-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3dff5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dff5-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="3dff5-126">Response</span></span>

<span data-ttu-id="3dff5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3dff5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dff5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3dff5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3dff5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3dff5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="3dff5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3dff5-131">Response</span></span>
<span data-ttu-id="3dff5-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3dff5-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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