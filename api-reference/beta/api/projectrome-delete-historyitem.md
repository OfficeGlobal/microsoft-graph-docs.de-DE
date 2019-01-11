---
title: Löschen einer historyItem
description: Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.
localization_priority: Normal
ms.openlocfilehash: d9468034f3a98e949eeb9f2da28c4a74c42cd991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834979"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="7ad8f-103">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="7ad8f-103">Delete a historyItem</span></span>

> <span data-ttu-id="7ad8f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ad8f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ad8f-106">Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-106">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ad8f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ad8f-107">Permissions</span></span>

<span data-ttu-id="7ad8f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ad8f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ad8f-110">Permission type</span></span>      | <span data-ttu-id="7ad8f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ad8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ad8f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ad8f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ad8f-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7ad8f-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7ad8f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ad8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ad8f-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7ad8f-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7ad8f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ad8f-116">Application</span></span> | <span data-ttu-id="7ad8f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ad8f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ad8f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad8f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ad8f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ad8f-119">Request headers</span></span>

|<span data-ttu-id="7ad8f-120">Name</span><span class="sxs-lookup"><span data-stu-id="7ad8f-120">Name</span></span> | <span data-ttu-id="7ad8f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7ad8f-121">Type</span></span> | <span data-ttu-id="7ad8f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad8f-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7ad8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad8f-123">Authorization</span></span> | <span data-ttu-id="7ad8f-124">string</span><span class="sxs-lookup"><span data-stu-id="7ad8f-124">string</span></span> | <span data-ttu-id="7ad8f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ad8f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ad8f-127">Request body</span></span>

<span data-ttu-id="7ad8f-128">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="7ad8f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad8f-129">Response</span></span>

<span data-ttu-id="7ad8f-130">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn das Historienelement gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-130">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="7ad8f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ad8f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ad8f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad8f-132">Request</span></span>

<span data-ttu-id="7ad8f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="7ad8f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad8f-134">Response</span></span>

<span data-ttu-id="7ad8f-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ad8f-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
