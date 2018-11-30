---
title: Löschen von groupLifecyclePolicy
description: Löscht groupLifecyclePolicy.
ms.openlocfilehash: 0e291ec0d05f03153f18974ad0aad29f2a8a86d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058938"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="f6c02-103">Löschen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f6c02-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="f6c02-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6c02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6c02-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6c02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6c02-106">Löscht [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f6c02-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c02-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f6c02-107">Permissions</span></span>

<span data-ttu-id="f6c02-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c02-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6c02-110">Permission type</span></span>      | <span data-ttu-id="f6c02-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6c02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6c02-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6c02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f6c02-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c02-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6c02-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6c02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c02-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6c02-115">Not supported</span></span> |
|<span data-ttu-id="f6c02-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6c02-116">Application</span></span> | <span data-ttu-id="f6c02-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c02-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6c02-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6c02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="f6c02-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6c02-119">Request headers</span></span>

| <span data-ttu-id="f6c02-120">Name</span><span class="sxs-lookup"><span data-stu-id="f6c02-120">Name</span></span> | <span data-ttu-id="f6c02-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6c02-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f6c02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c02-122">Authorization</span></span> | <span data-ttu-id="f6c02-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6c02-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6c02-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6c02-125">Content-Type</span></span>  | <span data-ttu-id="f6c02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6c02-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6c02-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6c02-127">Request body</span></span>
<span data-ttu-id="f6c02-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6c02-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f6c02-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6c02-129">Response</span></span>

<span data-ttu-id="f6c02-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6c02-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c02-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6c02-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6c02-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6c02-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="f6c02-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6c02-134">Response</span></span>

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