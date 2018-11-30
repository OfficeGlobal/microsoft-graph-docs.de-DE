---
title: Aktivität löschen
description: Löschen einer vorhandenen Benutzeraktivität für Ihre app.
ms.openlocfilehash: 9cdd52a2d3f417828e63107465dc28a4791a02e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062847"
---
# <a name="delete-an-activity"></a><span data-ttu-id="4650b-103">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="4650b-103">Delete an activity</span></span>

> <span data-ttu-id="4650b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4650b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4650b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4650b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4650b-106">Löschen einer vorhandenen Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="4650b-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="4650b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4650b-107">Permissions</span></span>

<span data-ttu-id="4650b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4650b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4650b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4650b-110">Permission type</span></span>      | <span data-ttu-id="4650b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4650b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4650b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4650b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4650b-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4650b-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4650b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4650b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4650b-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4650b-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4650b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4650b-116">Application</span></span> | <span data-ttu-id="4650b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4650b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4650b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4650b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4650b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4650b-119">Request headers</span></span>

|<span data-ttu-id="4650b-120">Name</span><span class="sxs-lookup"><span data-stu-id="4650b-120">Name</span></span> | <span data-ttu-id="4650b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4650b-121">Type</span></span> | <span data-ttu-id="4650b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4650b-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4650b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4650b-123">Authorization</span></span> | <span data-ttu-id="4650b-124">string</span><span class="sxs-lookup"><span data-stu-id="4650b-124">string</span></span> | <span data-ttu-id="4650b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4650b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4650b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4650b-127">Request body</span></span>

<span data-ttu-id="4650b-128">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="4650b-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="4650b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4650b-129">Response</span></span>

<span data-ttu-id="4650b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn die Aktivität gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="4650b-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="4650b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4650b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4650b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4650b-132">Request</span></span>

<span data-ttu-id="4650b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4650b-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="4650b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4650b-134">Response</span></span>

<span data-ttu-id="4650b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4650b-135">Here is an example of the response.</span></span>

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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->