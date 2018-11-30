---
title: Aktivität löschen
description: Löschen einer vorhandenen Benutzeraktivität für Ihre app.
ms.openlocfilehash: a4b32e00719772f6dcfb715fa69350edf9a8b48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016908"
---
# <a name="delete-an-activity"></a><span data-ttu-id="198df-103">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="198df-103">Delete an activity</span></span>

<span data-ttu-id="198df-104">Löschen einer vorhandenen Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="198df-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="198df-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="198df-105">Permissions</span></span>

<span data-ttu-id="198df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="198df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="198df-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="198df-108">Permission type</span></span>      | <span data-ttu-id="198df-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="198df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="198df-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="198df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="198df-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="198df-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="198df-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="198df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="198df-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="198df-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="198df-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="198df-114">Application</span></span> | <span data-ttu-id="198df-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="198df-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="198df-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="198df-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="198df-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="198df-117">Request headers</span></span>

|<span data-ttu-id="198df-118">Name</span><span class="sxs-lookup"><span data-stu-id="198df-118">Name</span></span> | <span data-ttu-id="198df-119">Typ</span><span class="sxs-lookup"><span data-stu-id="198df-119">Type</span></span> | <span data-ttu-id="198df-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="198df-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="198df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="198df-121">Authorization</span></span> | <span data-ttu-id="198df-122">string</span><span class="sxs-lookup"><span data-stu-id="198df-122">string</span></span> | <span data-ttu-id="198df-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="198df-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="198df-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="198df-125">Request body</span></span>

<span data-ttu-id="198df-126">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="198df-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="198df-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="198df-127">Response</span></span>

<span data-ttu-id="198df-128">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn die Aktivität gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="198df-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="198df-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="198df-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="198df-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="198df-130">Request</span></span>

<span data-ttu-id="198df-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="198df-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="198df-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="198df-132">Response</span></span>

<span data-ttu-id="198df-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="198df-133">Here is an example of the response.</span></span>

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