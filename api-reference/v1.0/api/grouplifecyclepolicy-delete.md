---
title: Löschen von groupLifecyclePolicy
description: Löscht groupLifecyclePolicy.
author: dkershaw10
ms.openlocfilehash: 606b8f5406277dbde34ca731c374a064b552ac97
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351590"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="0cf01-103">Löschen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0cf01-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="0cf01-104">Löscht [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0cf01-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf01-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0cf01-105">Permissions</span></span>

<span data-ttu-id="0cf01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf01-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0cf01-108">Permission type</span></span>      | <span data-ttu-id="0cf01-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0cf01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cf01-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0cf01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cf01-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf01-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cf01-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0cf01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cf01-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cf01-113">Not supported.</span></span>    |
|<span data-ttu-id="0cf01-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0cf01-114">Application</span></span> | <span data-ttu-id="0cf01-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf01-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cf01-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cf01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="0cf01-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0cf01-117">Request headers</span></span>

| <span data-ttu-id="0cf01-118">Name</span><span class="sxs-lookup"><span data-stu-id="0cf01-118">Name</span></span> | <span data-ttu-id="0cf01-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cf01-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="0cf01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf01-120">Authorization</span></span> | <span data-ttu-id="0cf01-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0cf01-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0cf01-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cf01-123">Content-Type</span></span>  | <span data-ttu-id="0cf01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0cf01-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cf01-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0cf01-125">Request body</span></span>
<span data-ttu-id="0cf01-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0cf01-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0cf01-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cf01-127">Response</span></span>

<span data-ttu-id="0cf01-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0cf01-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf01-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0cf01-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0cf01-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cf01-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="0cf01-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cf01-132">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->