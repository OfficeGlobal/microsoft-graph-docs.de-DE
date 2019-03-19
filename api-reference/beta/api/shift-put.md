---
title: UMSCHALT ersetzen
description: Ersetzen Sie eine vorhandene Schicht.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d8614739757e3962e671440a9a893b9b06d6761f
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657847"
---
# <a name="replace-shift"></a><span data-ttu-id="225e5-103">UMSCHALT ersetzen</span><span class="sxs-lookup"><span data-stu-id="225e5-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="225e5-104">Ersetzen Sie eine vorhandene [Schicht](../resources/shift.md).</span><span class="sxs-lookup"><span data-stu-id="225e5-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="225e5-105">Wenn die angegebene [Schicht](../resources/shift.md) nicht vorhanden ist, gibt diese `404 Not found`Methode zurück.</span><span class="sxs-lookup"><span data-stu-id="225e5-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="225e5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="225e5-106">Permissions</span></span>

<span data-ttu-id="225e5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225e5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="225e5-109">Permission type</span></span>      | <span data-ttu-id="225e5-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="225e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="225e5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="225e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="225e5-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225e5-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="225e5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="225e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="225e5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="225e5-114">Not supported.</span></span>    |
|<span data-ttu-id="225e5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="225e5-115">Application</span></span> | <span data-ttu-id="225e5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="225e5-116">Not supported.</span></span> |

> <span data-ttu-id="225e5-117">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="225e5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="225e5-118">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="225e5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="225e5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="225e5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="225e5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="225e5-120">Request headers</span></span>

| <span data-ttu-id="225e5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="225e5-121">Header</span></span>       | <span data-ttu-id="225e5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="225e5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="225e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="225e5-123">Authorization</span></span>  | <span data-ttu-id="225e5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="225e5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="225e5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="225e5-126">Content-Type</span></span>  | <span data-ttu-id="225e5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="225e5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="225e5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="225e5-128">Request body</span></span>

<span data-ttu-id="225e5-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [Shift](../resources/shift.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="225e5-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="225e5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="225e5-130">Response</span></span>

<span data-ttu-id="225e5-131">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Shift](../resources/shift.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="225e5-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="225e5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="225e5-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="225e5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="225e5-133">Request</span></span>

<span data-ttu-id="225e5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="225e5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

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

#### <a name="response"></a><span data-ttu-id="225e5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="225e5-135">Response</span></span>

<span data-ttu-id="225e5-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="225e5-136">The following is an example of the response.</span></span> 

><span data-ttu-id="225e5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="225e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->