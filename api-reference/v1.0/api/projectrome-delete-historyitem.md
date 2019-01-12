---
title: Löschen einer historyItem
description: Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 4814987367b7b9a278c645dbdca8fb5e795ce784
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923936"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="9aa13-103">Löschen einer historyItem</span><span class="sxs-lookup"><span data-stu-id="9aa13-103">Delete a historyItem</span></span>

<span data-ttu-id="9aa13-104">Löschen Sie ein vorhandenes Verlaufselement für einen vorhandenen Benutzer-Aktivität hinzu.</span><span class="sxs-lookup"><span data-stu-id="9aa13-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="9aa13-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9aa13-105">Permissions</span></span>

<span data-ttu-id="9aa13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aa13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9aa13-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9aa13-108">Permission type</span></span>      | <span data-ttu-id="9aa13-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9aa13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9aa13-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9aa13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9aa13-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9aa13-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9aa13-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9aa13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9aa13-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9aa13-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9aa13-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9aa13-114">Application</span></span> | <span data-ttu-id="9aa13-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9aa13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9aa13-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9aa13-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9aa13-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9aa13-117">Request headers</span></span>

|<span data-ttu-id="9aa13-118">Name</span><span class="sxs-lookup"><span data-stu-id="9aa13-118">Name</span></span> | <span data-ttu-id="9aa13-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9aa13-119">Type</span></span> | <span data-ttu-id="9aa13-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9aa13-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="9aa13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aa13-121">Authorization</span></span> | <span data-ttu-id="9aa13-122">string</span><span class="sxs-lookup"><span data-stu-id="9aa13-122">string</span></span> | <span data-ttu-id="9aa13-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9aa13-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aa13-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9aa13-125">Request body</span></span>

<span data-ttu-id="9aa13-126">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="9aa13-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="9aa13-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9aa13-127">Response</span></span>

<span data-ttu-id="9aa13-128">Wenn der Vorgang erfolgreich war, gibt diese Methode die `204 No Content` Antwortcode, wenn das Historienelement gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="9aa13-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="9aa13-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9aa13-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9aa13-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9aa13-130">Request</span></span>

<span data-ttu-id="9aa13-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9aa13-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="9aa13-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9aa13-132">Response</span></span>

<span data-ttu-id="9aa13-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9aa13-133">Here is an example of the response.</span></span>

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
