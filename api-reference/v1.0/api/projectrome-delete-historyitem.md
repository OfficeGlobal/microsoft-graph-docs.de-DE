---
title: Löschen einer historyItem
description: Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.
localization_priority: Normal
ms.openlocfilehash: 3476aba19a2de09f5b4c168ab2a4075b74fd2a93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861922"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="87243-103">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="87243-103">Delete a historyItem</span></span>

<span data-ttu-id="87243-104">Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.</span><span class="sxs-lookup"><span data-stu-id="87243-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="87243-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87243-105">Permissions</span></span>

<span data-ttu-id="87243-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87243-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87243-108">Permission type</span></span>      | <span data-ttu-id="87243-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87243-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87243-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87243-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87243-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87243-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87243-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87243-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87243-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87243-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87243-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87243-114">Application</span></span> | <span data-ttu-id="87243-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87243-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87243-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87243-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87243-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87243-117">Request headers</span></span>

|<span data-ttu-id="87243-118">Name</span><span class="sxs-lookup"><span data-stu-id="87243-118">Name</span></span> | <span data-ttu-id="87243-119">Typ</span><span class="sxs-lookup"><span data-stu-id="87243-119">Type</span></span> | <span data-ttu-id="87243-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87243-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="87243-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87243-121">Authorization</span></span> | <span data-ttu-id="87243-122">string</span><span class="sxs-lookup"><span data-stu-id="87243-122">string</span></span> | <span data-ttu-id="87243-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87243-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87243-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87243-125">Request body</span></span>

<span data-ttu-id="87243-126">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="87243-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="87243-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="87243-127">Response</span></span>

<span data-ttu-id="87243-128">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn das Historienelement gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="87243-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="87243-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87243-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87243-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87243-130">Request</span></span>

<span data-ttu-id="87243-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87243-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="87243-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="87243-132">Response</span></span>

<span data-ttu-id="87243-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87243-133">Here is an example of the response.</span></span>

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
