---
title: Aktivität löschen
description: Löschen einer vorhandenen Benutzeraktivität für Ihre app.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 8b4bf0b09cb5796e1db8e22ced7e471bdd5117f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925749"
---
# <a name="delete-an-activity"></a><span data-ttu-id="e9131-103">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="e9131-103">Delete an activity</span></span>

> <span data-ttu-id="e9131-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e9131-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9131-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9131-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9131-106">Löschen einer vorhandenen Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="e9131-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9131-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e9131-107">Permissions</span></span>

<span data-ttu-id="e9131-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9131-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9131-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9131-110">Permission type</span></span>      | <span data-ttu-id="e9131-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9131-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9131-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9131-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9131-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e9131-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e9131-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9131-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9131-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e9131-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e9131-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9131-116">Application</span></span> | <span data-ttu-id="e9131-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9131-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9131-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9131-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e9131-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9131-119">Request headers</span></span>

|<span data-ttu-id="e9131-120">Name</span><span class="sxs-lookup"><span data-stu-id="e9131-120">Name</span></span> | <span data-ttu-id="e9131-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e9131-121">Type</span></span> | <span data-ttu-id="e9131-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9131-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e9131-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9131-123">Authorization</span></span> | <span data-ttu-id="e9131-124">string</span><span class="sxs-lookup"><span data-stu-id="e9131-124">string</span></span> | <span data-ttu-id="e9131-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e9131-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9131-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9131-127">Request body</span></span>

<span data-ttu-id="e9131-128">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="e9131-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="e9131-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9131-129">Response</span></span>

<span data-ttu-id="e9131-130">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn die Aktivität gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="e9131-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="e9131-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9131-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e9131-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9131-132">Request</span></span>

<span data-ttu-id="e9131-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9131-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="e9131-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9131-134">Response</span></span>

<span data-ttu-id="e9131-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e9131-135">Here is an example of the response.</span></span>

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
