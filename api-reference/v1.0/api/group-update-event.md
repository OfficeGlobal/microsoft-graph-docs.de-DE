---
title: Ereignis aktualisieren
description: Aktualisieren eines event-Objekts.
author: dkershaw10
ms.openlocfilehash: c8aacc7df62bf336c355801e89e1b6bea5c2b1f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321161"
---
# <a name="update-event"></a><span data-ttu-id="26923-103">Ereignis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="26923-103">Update event</span></span>
<span data-ttu-id="26923-104">Aktualisieren eines [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="26923-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26923-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="26923-105">Permissions</span></span>
<span data-ttu-id="26923-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26923-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26923-108">Permission type</span></span>      | <span data-ttu-id="26923-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26923-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26923-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26923-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26923-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26923-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26923-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26923-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26923-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26923-113">Not supported.</span></span>    |
|<span data-ttu-id="26923-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26923-114">Application</span></span> | <span data-ttu-id="26923-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26923-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26923-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26923-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26923-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26923-117">Request headers</span></span>
| <span data-ttu-id="26923-118">Name</span><span class="sxs-lookup"><span data-stu-id="26923-118">Name</span></span>       | <span data-ttu-id="26923-119">Typ</span><span class="sxs-lookup"><span data-stu-id="26923-119">Type</span></span> | <span data-ttu-id="26923-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26923-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26923-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="26923-121">Authorization</span></span>  | <span data-ttu-id="26923-122">string</span><span class="sxs-lookup"><span data-stu-id="26923-122">string</span></span>  | <span data-ttu-id="26923-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="26923-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26923-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26923-125">Request body</span></span>
<span data-ttu-id="26923-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="26923-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="26923-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="26923-129">Response</span></span>
<span data-ttu-id="26923-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26923-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26923-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26923-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="26923-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26923-132">Request</span></span>
<span data-ttu-id="26923-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26923-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="26923-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="26923-134">Response</span></span>
<span data-ttu-id="26923-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="26923-135">The following is an example of the response.</span></span>

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