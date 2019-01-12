---
title: Anruf löschen
description: Löschen oder einen aktiven Anruf Auflegen.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0163f7eee4933406999e283378f31d7f5aeb92b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946765"
---
# <a name="delete-call"></a><span data-ttu-id="d12aa-103">Anruf löschen</span><span class="sxs-lookup"><span data-stu-id="d12aa-103">Delete call</span></span>

> <span data-ttu-id="d12aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d12aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d12aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d12aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d12aa-106">Löschen oder einen aktiven Anruf Auflegen.</span><span class="sxs-lookup"><span data-stu-id="d12aa-106">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d12aa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d12aa-107">Permissions</span></span>

<span data-ttu-id="d12aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d12aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d12aa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d12aa-110">Permission type</span></span> | <span data-ttu-id="d12aa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d12aa-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d12aa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d12aa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d12aa-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d12aa-113">Not Supported.</span></span>                         |
| <span data-ttu-id="d12aa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d12aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d12aa-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d12aa-115">Not Supported.</span></span>                         |
| <span data-ttu-id="d12aa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d12aa-116">Application</span></span>                            | <span data-ttu-id="d12aa-117">Keine.</span><span class="sxs-lookup"><span data-stu-id="d12aa-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d12aa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d12aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d12aa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d12aa-119">Request headers</span></span>
| <span data-ttu-id="d12aa-120">Name</span><span class="sxs-lookup"><span data-stu-id="d12aa-120">Name</span></span>          | <span data-ttu-id="d12aa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d12aa-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d12aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d12aa-122">Authorization</span></span> | <span data-ttu-id="d12aa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d12aa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d12aa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d12aa-125">Request body</span></span>
<span data-ttu-id="d12aa-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d12aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d12aa-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d12aa-127">Response</span></span>
<span data-ttu-id="d12aa-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d12aa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d12aa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d12aa-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d12aa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d12aa-131">Request</span></span>
<span data-ttu-id="d12aa-132">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="d12aa-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="d12aa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d12aa-133">Response</span></span>

> <span data-ttu-id="d12aa-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d12aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="d12aa-136">Benachrichtigung - beenden</span><span class="sxs-lookup"><span data-stu-id="d12aa-136">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="d12aa-137">Benachrichtigung - beendet</span><span class="sxs-lookup"><span data-stu-id="d12aa-137">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
