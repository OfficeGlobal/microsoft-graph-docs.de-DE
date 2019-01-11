---
title: Aktivität löschen
description: Löschen einer vorhandenen Benutzeraktivität für Ihre app.
localization_priority: Normal
ms.openlocfilehash: fab008e9a9d031aed12605f14bf447247c0227ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838150"
---
# <a name="delete-an-activity"></a><span data-ttu-id="abef0-103">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="abef0-103">Delete an activity</span></span>

<span data-ttu-id="abef0-104">Löschen einer vorhandenen Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="abef0-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="abef0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="abef0-105">Permissions</span></span>

<span data-ttu-id="abef0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="abef0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abef0-108">Permission type</span></span>      | <span data-ttu-id="abef0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abef0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abef0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abef0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abef0-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="abef0-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="abef0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abef0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abef0-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="abef0-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="abef0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abef0-114">Application</span></span> | <span data-ttu-id="abef0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abef0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abef0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abef0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="abef0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abef0-117">Request headers</span></span>

|<span data-ttu-id="abef0-118">Name</span><span class="sxs-lookup"><span data-stu-id="abef0-118">Name</span></span> | <span data-ttu-id="abef0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="abef0-119">Type</span></span> | <span data-ttu-id="abef0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abef0-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="abef0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abef0-121">Authorization</span></span> | <span data-ttu-id="abef0-122">string</span><span class="sxs-lookup"><span data-stu-id="abef0-122">string</span></span> | <span data-ttu-id="abef0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="abef0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abef0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abef0-125">Request body</span></span>

<span data-ttu-id="abef0-126">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="abef0-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="abef0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="abef0-127">Response</span></span>

<span data-ttu-id="abef0-128">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn die Aktivität gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="abef0-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="abef0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abef0-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="abef0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abef0-130">Request</span></span>

<span data-ttu-id="abef0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abef0-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="abef0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="abef0-132">Response</span></span>

<span data-ttu-id="abef0-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="abef0-133">Here is an example of the response.</span></span>

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
