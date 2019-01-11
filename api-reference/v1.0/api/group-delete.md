---
title: Gruppe löschen
description: Mit dieser API können Sie Gruppen löschen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b9d2e9cbe3a86906c815178b570cd6d7980ac89e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808309"
---
# <a name="delete-group"></a><span data-ttu-id="b463c-103">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="b463c-103">Delete group</span></span>
<span data-ttu-id="b463c-104">Mit dieser API können Sie Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="b463c-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b463c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b463c-105">Permissions</span></span>
<span data-ttu-id="b463c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b463c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b463c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b463c-108">Permission type</span></span>      | <span data-ttu-id="b463c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b463c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b463c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b463c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b463c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b463c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b463c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b463c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b463c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b463c-113">Not supported.</span></span>    |
|<span data-ttu-id="b463c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b463c-114">Application</span></span> | <span data-ttu-id="b463c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b463c-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b463c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b463c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b463c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b463c-117">Request headers</span></span>
| <span data-ttu-id="b463c-118">Name</span><span class="sxs-lookup"><span data-stu-id="b463c-118">Name</span></span>       | <span data-ttu-id="b463c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b463c-119">Type</span></span> | <span data-ttu-id="b463c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b463c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b463c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b463c-121">Authorization</span></span>  | <span data-ttu-id="b463c-122">string</span><span class="sxs-lookup"><span data-stu-id="b463c-122">string</span></span>  | <span data-ttu-id="b463c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b463c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b463c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b463c-125">Request body</span></span>
<span data-ttu-id="b463c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b463c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b463c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b463c-127">Response</span></span>
<span data-ttu-id="b463c-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b463c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b463c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b463c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b463c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b463c-131">Request</span></span>
<span data-ttu-id="b463c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b463c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="b463c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b463c-133">Response</span></span>
<span data-ttu-id="b463c-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b463c-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
