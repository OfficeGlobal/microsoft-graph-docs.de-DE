---
title: Ereignis aktualisieren
description: Aktualisieren eines event-Objekts.
ms.openlocfilehash: 94dfa35e4b37e4e38746223604d3d3b3c7311a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062304"
---
# <a name="update-event"></a><span data-ttu-id="82688-103">Ereignis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="82688-103">Update event</span></span>

> <span data-ttu-id="82688-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="82688-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82688-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82688-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82688-106">Aktualisieren eines [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="82688-106">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82688-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82688-107">Permissions</span></span>
<span data-ttu-id="82688-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82688-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82688-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82688-110">Permission type</span></span>      | <span data-ttu-id="82688-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82688-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82688-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82688-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82688-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82688-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82688-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82688-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82688-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82688-115">Not supported.</span></span>    |
|<span data-ttu-id="82688-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82688-116">Application</span></span> | <span data-ttu-id="82688-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82688-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82688-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82688-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="82688-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82688-119">Request headers</span></span>
| <span data-ttu-id="82688-120">Name</span><span class="sxs-lookup"><span data-stu-id="82688-120">Name</span></span>       | <span data-ttu-id="82688-121">Typ</span><span class="sxs-lookup"><span data-stu-id="82688-121">Type</span></span> | <span data-ttu-id="82688-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82688-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82688-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82688-123">Authorization</span></span>  | <span data-ttu-id="82688-124">string</span><span class="sxs-lookup"><span data-stu-id="82688-124">string</span></span>  | <span data-ttu-id="82688-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82688-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82688-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82688-127">Request body</span></span>
<span data-ttu-id="82688-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="82688-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="82688-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="82688-131">Response</span></span>
<span data-ttu-id="82688-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82688-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="82688-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82688-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82688-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82688-134">Request</span></span>
<span data-ttu-id="82688-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82688-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="82688-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="82688-136">Response</span></span>
<span data-ttu-id="82688-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82688-137">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->