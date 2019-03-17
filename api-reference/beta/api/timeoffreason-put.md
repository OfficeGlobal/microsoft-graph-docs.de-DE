---
title: TimeOffReason ersetzen
description: Ersetzen eines vorhandenen timeOffReason.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8c37304d6556bfcee47a0bb631933f29cd8b3986
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657812"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="49f64-103">TimeOffReason ersetzen</span><span class="sxs-lookup"><span data-stu-id="49f64-103">Replace timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f64-104">Ersetzen eines vorhandenen [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="49f64-104">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="49f64-105">Wenn die angegebene [timeOffReason](../resources/timeoffreason.md) nicht vorhanden ist, gibt diese `404 Not found`Methode zurück.</span><span class="sxs-lookup"><span data-stu-id="49f64-105">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="49f64-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49f64-106">Permissions</span></span>

<span data-ttu-id="49f64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f64-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49f64-109">Permission type</span></span>      | <span data-ttu-id="49f64-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49f64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f64-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49f64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49f64-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f64-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49f64-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49f64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f64-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49f64-114">Not supported.</span></span>    |
|<span data-ttu-id="49f64-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49f64-115">Application</span></span> | <span data-ttu-id="49f64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49f64-116">Not supported.</span></span> |

> <span data-ttu-id="49f64-117">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="49f64-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="49f64-118">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="49f64-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="49f64-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49f64-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="49f64-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49f64-120">Request headers</span></span>

| <span data-ttu-id="49f64-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="49f64-121">Header</span></span>       | <span data-ttu-id="49f64-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49f64-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49f64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49f64-123">Authorization</span></span>  | <span data-ttu-id="49f64-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f64-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49f64-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49f64-126">Content-Type</span></span>  | <span data-ttu-id="49f64-127">application/json</span><span class="sxs-lookup"><span data-stu-id="49f64-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49f64-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49f64-128">Request body</span></span>

<span data-ttu-id="49f64-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [timeOffReason](../resources/timeoffreason.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="49f64-129">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="49f64-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="49f64-130">Response</span></span>

<span data-ttu-id="49f64-131">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [timeOffReason](../resources/timeoffreason.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="49f64-131">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f64-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49f64-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="49f64-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49f64-133">Request</span></span>

<span data-ttu-id="49f64-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49f64-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```

#### <a name="response"></a><span data-ttu-id="49f64-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="49f64-135">Response</span></span>

<span data-ttu-id="49f64-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="49f64-136">The following is an example of the response.</span></span> 

><span data-ttu-id="49f64-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="49f64-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
