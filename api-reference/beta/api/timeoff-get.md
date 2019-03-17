---
title: TimeOff abrufen
description: Rufen Sie eine timeOff nach ID ab.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8408fc1c83668b5f3bc6f6086b97915854b7d255
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657497"
---
# <a name="get-timeoff"></a><span data-ttu-id="d48d9-103">TimeOff abrufen</span><span class="sxs-lookup"><span data-stu-id="d48d9-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d48d9-104">Ruft die Eigenschaften und Beziehungen eines [TIMEOFF](../resources/timeoff.md) -Objekts anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="d48d9-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d48d9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d48d9-105">Permissions</span></span>

<span data-ttu-id="d48d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d48d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d48d9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d48d9-108">Permission type</span></span>      | <span data-ttu-id="d48d9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d48d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d48d9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d48d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d48d9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d48d9-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d48d9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d48d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d48d9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d48d9-113">Not supported.</span></span>    |
|<span data-ttu-id="d48d9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d48d9-114">Application</span></span> | <span data-ttu-id="d48d9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d48d9-115">Not supported.</span></span> |

> <span data-ttu-id="d48d9-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d48d9-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d48d9-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="d48d9-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d48d9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d48d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="d48d9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d48d9-119">Request headers</span></span>

| <span data-ttu-id="d48d9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d48d9-120">Header</span></span>       | <span data-ttu-id="d48d9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d48d9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d48d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d48d9-122">Authorization</span></span>  | <span data-ttu-id="d48d9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d48d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d48d9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d48d9-125">Content-Type</span></span>  | <span data-ttu-id="d48d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d48d9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d48d9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d48d9-127">Request body</span></span>
<span data-ttu-id="d48d9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d48d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d48d9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d48d9-129">Response</span></span>

<span data-ttu-id="d48d9-130">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [timeOff](../resources/timeoff.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d48d9-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d48d9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d48d9-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d48d9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d48d9-132">Request</span></span>

<span data-ttu-id="d48d9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d48d9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="d48d9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d48d9-134">Response</span></span>

<span data-ttu-id="d48d9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d48d9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="d48d9-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d48d9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
