---
title: TimeOff erstellen
description: Erstellen Sie eine neue timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: df954be9d07797e663b205af6d4dc1ef5dfb20ff
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657504"
---
# <a name="create-timeoff"></a><span data-ttu-id="7c964-103">TimeOff erstellen</span><span class="sxs-lookup"><span data-stu-id="7c964-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c964-104">Erstellen Sie eine neue [timeOff](../resources/timeoff.md) -Instanz in einem [Zeitplan](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="7c964-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c964-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c964-105">Permissions</span></span>

<span data-ttu-id="7c964-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c964-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c964-108">Permission type</span></span>      | <span data-ttu-id="7c964-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c964-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c964-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c964-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c964-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c964-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c964-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c964-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c964-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c964-113">Not supported.</span></span>    |
|<span data-ttu-id="7c964-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c964-114">Application</span></span> | <span data-ttu-id="7c964-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c964-115">Not supported.</span></span> |

> <span data-ttu-id="7c964-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="7c964-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7c964-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="7c964-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c964-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c964-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="7c964-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c964-119">Request headers</span></span>

| <span data-ttu-id="7c964-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c964-120">Header</span></span>       | <span data-ttu-id="7c964-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7c964-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c964-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c964-122">Authorization</span></span>  | <span data-ttu-id="7c964-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c964-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c964-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c964-125">Content-Type</span></span>  | <span data-ttu-id="7c964-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c964-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="7c964-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c964-127">Response</span></span>

<span data-ttu-id="7c964-128">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [timeOff](../resources/timeoff.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c964-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c964-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c964-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c964-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c964-130">Request</span></span>

<span data-ttu-id="7c964-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c964-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

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

#### <a name="response"></a><span data-ttu-id="7c964-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c964-132">Response</span></span>

<span data-ttu-id="7c964-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c964-133">The following is an example of the response.</span></span> 

><span data-ttu-id="7c964-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7c964-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "schedule-post-timesoff"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-timesoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
