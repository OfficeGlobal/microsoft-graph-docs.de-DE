---
title: Unterhaltungsthread aktualisieren
description: Aktualisieren eines Thread-Objekts.
ms.openlocfilehash: e66a65c42a3616968f528ba3c2a1dda0d160e7f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018141"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="a7c0b-103">Unterhaltungsthread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a7c0b-103">Update conversation thread</span></span>
<span data-ttu-id="a7c0b-104">Aktualisieren eines [Thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-104">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7c0b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a7c0b-105">Permissions</span></span>
<span data-ttu-id="a7c0b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c0b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7c0b-108">Permission type</span></span>      | <span data-ttu-id="a7c0b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7c0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7c0b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7c0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7c0b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7c0b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7c0b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7c0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7c0b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7c0b-113">Not supported.</span></span>    |
|<span data-ttu-id="a7c0b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7c0b-114">Application</span></span> | <span data-ttu-id="a7c0b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7c0b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7c0b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7c0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7c0b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7c0b-117">Request headers</span></span>
| <span data-ttu-id="a7c0b-118">Name</span><span class="sxs-lookup"><span data-stu-id="a7c0b-118">Name</span></span>       | <span data-ttu-id="a7c0b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a7c0b-119">Type</span></span> | <span data-ttu-id="a7c0b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7c0b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7c0b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7c0b-121">Authorization</span></span>  | <span data-ttu-id="a7c0b-122">string</span><span class="sxs-lookup"><span data-stu-id="a7c0b-122">string</span></span>  | <span data-ttu-id="a7c0b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7c0b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7c0b-125">Request body</span></span>
<span data-ttu-id="a7c0b-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a7c0b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7c0b-129">Response</span></span>
<span data-ttu-id="a7c0b-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7c0b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7c0b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a7c0b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7c0b-132">Request</span></span>
<span data-ttu-id="a7c0b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="a7c0b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7c0b-134">Response</span></span>
<span data-ttu-id="a7c0b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a7c0b-135">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->