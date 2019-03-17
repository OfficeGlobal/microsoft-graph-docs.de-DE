---
title: TimeOff ersetzen
description: Ersetzen eines vorhandenen timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: baa95edcece586a481a538d2f0ff68a309c8ce10
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657693"
---
# <a name="replace-timeoff"></a><span data-ttu-id="e4cf3-103">TimeOff ersetzen</span><span class="sxs-lookup"><span data-stu-id="e4cf3-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4cf3-104">Ersetzen eines vorhandenen [timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="e4cf3-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="e4cf3-105">Wenn die angegebene [timeOff](../resources/timeoff.md) nicht vorhanden ist, gibt diese `404 Not found`Methode zurück.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4cf3-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4cf3-106">Permissions</span></span>

<span data-ttu-id="e4cf3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4cf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4cf3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4cf3-109">Permission type</span></span>      | <span data-ttu-id="e4cf3-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4cf3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4cf3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4cf3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4cf3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4cf3-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4cf3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4cf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4cf3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4cf3-114">Not supported.</span></span>    |
|<span data-ttu-id="e4cf3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4cf3-115">Application</span></span> | <span data-ttu-id="e4cf3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4cf3-116">Not supported.</span></span> |

> <span data-ttu-id="e4cf3-117">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e4cf3-118">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e4cf3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4cf3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="e4cf3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4cf3-120">Request headers</span></span>

| <span data-ttu-id="e4cf3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4cf3-121">Header</span></span>       | <span data-ttu-id="e4cf3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4cf3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4cf3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4cf3-123">Authorization</span></span>  | <span data-ttu-id="e4cf3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4cf3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4cf3-126">Content-Type</span></span>  | <span data-ttu-id="e4cf3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e4cf3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4cf3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4cf3-128">Request body</span></span>

<span data-ttu-id="e4cf3-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [timeOff](../resources/timeoff.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e4cf3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4cf3-130">Response</span></span>

<span data-ttu-id="e4cf3-131">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [timeOff](../resources/timeoff.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4cf3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4cf3-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e4cf3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4cf3-133">Request</span></span>

<span data-ttu-id="e4cf3-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

#### <a name="response"></a><span data-ttu-id="e4cf3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4cf3-135">Response</span></span>

<span data-ttu-id="e4cf3-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-136">The following is an example of the response.</span></span> 

><span data-ttu-id="e4cf3-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e4cf3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
