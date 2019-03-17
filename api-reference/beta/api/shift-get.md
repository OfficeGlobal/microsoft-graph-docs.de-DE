---
title: Shift abrufen
description: Eine Schicht nach ID erhalten.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 60d2aa9c09305ee016d16d15514e14d91cf7a5cc
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657861"
---
# <a name="get-shift"></a><span data-ttu-id="5555b-103">Shift abrufen</span><span class="sxs-lookup"><span data-stu-id="5555b-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5555b-104">Ruft die Eigenschaften und Beziehungen eines [Shift](../resources/shift.md) -Objekts anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="5555b-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="5555b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5555b-105">Permissions</span></span>

<span data-ttu-id="5555b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5555b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5555b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5555b-108">Permission type</span></span>      | <span data-ttu-id="5555b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5555b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5555b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5555b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5555b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5555b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5555b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5555b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5555b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5555b-113">Not supported.</span></span>    |
|<span data-ttu-id="5555b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5555b-114">Application</span></span> | <span data-ttu-id="5555b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5555b-115">Not supported.</span></span> |

> <span data-ttu-id="5555b-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="5555b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5555b-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="5555b-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5555b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5555b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="5555b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5555b-119">Request headers</span></span>

| <span data-ttu-id="5555b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5555b-120">Header</span></span>       | <span data-ttu-id="5555b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5555b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5555b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5555b-122">Authorization</span></span>  | <span data-ttu-id="5555b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5555b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5555b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5555b-125">Content-Type</span></span>  | <span data-ttu-id="5555b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5555b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5555b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5555b-127">Request body</span></span>
<span data-ttu-id="5555b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5555b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5555b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5555b-129">Response</span></span>

<span data-ttu-id="5555b-130">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Shift](../resources/shift.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5555b-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5555b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5555b-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5555b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5555b-132">Request</span></span>

<span data-ttu-id="5555b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5555b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="5555b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5555b-134">Response</span></span>

<span data-ttu-id="5555b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5555b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5555b-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5555b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
