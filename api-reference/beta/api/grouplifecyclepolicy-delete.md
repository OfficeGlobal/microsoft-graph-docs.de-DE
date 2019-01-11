---
title: Löschen von groupLifecyclePolicy
description: Löscht groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f92a8fbfd0a45abfdfbb1705f99eaa2d7335bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882579"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="db27f-103">Löschen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="db27f-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="db27f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db27f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db27f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db27f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db27f-106">Löscht [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="db27f-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db27f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db27f-107">Permissions</span></span>

<span data-ttu-id="db27f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db27f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db27f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db27f-110">Permission type</span></span>      | <span data-ttu-id="db27f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db27f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db27f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db27f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db27f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db27f-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="db27f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db27f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db27f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db27f-115">Not supported</span></span> |
|<span data-ttu-id="db27f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db27f-116">Application</span></span> | <span data-ttu-id="db27f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db27f-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db27f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db27f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="db27f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db27f-119">Request headers</span></span>

| <span data-ttu-id="db27f-120">Name</span><span class="sxs-lookup"><span data-stu-id="db27f-120">Name</span></span> | <span data-ttu-id="db27f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db27f-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="db27f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db27f-122">Authorization</span></span> | <span data-ttu-id="db27f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db27f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db27f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db27f-125">Content-Type</span></span>  | <span data-ttu-id="db27f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db27f-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="db27f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db27f-127">Request body</span></span>
<span data-ttu-id="db27f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="db27f-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="db27f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="db27f-129">Response</span></span>

<span data-ttu-id="db27f-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db27f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db27f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db27f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db27f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db27f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="db27f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="db27f-134">Response</span></span>

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
