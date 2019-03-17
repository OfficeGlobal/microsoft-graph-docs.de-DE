---
title: Listen Verschiebungen
description: Rufen Sie die Liste der Schichten in einem Zeitplan ab.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1250ac0d05636d83602412c912bff604938a317a
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657777"
---
# <a name="list-shifts"></a><span data-ttu-id="6c69e-103">Listen Verschiebungen</span><span class="sxs-lookup"><span data-stu-id="6c69e-103">List shifts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6c69e-104">Rufen Sie die Liste der [Shift](../resources/shift.md) -Instanzen in einem [Zeitplan](../resources/schedule.md)ab.</span><span class="sxs-lookup"><span data-stu-id="6c69e-104">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c69e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6c69e-105">Permissions</span></span>

<span data-ttu-id="6c69e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c69e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c69e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c69e-108">Permission type</span></span>      | <span data-ttu-id="6c69e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c69e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c69e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c69e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c69e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c69e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c69e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c69e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c69e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c69e-113">Not supported.</span></span>    |
|<span data-ttu-id="6c69e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c69e-114">Application</span></span> | <span data-ttu-id="6c69e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c69e-115">Not supported.</span></span> |

> <span data-ttu-id="6c69e-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="6c69e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6c69e-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="6c69e-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c69e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c69e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c69e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6c69e-119">Optional query parameters</span></span>
<span data-ttu-id="6c69e-120">Diese Methode unterstützt den $filter [OData-Abfrageparameter](/graph/query-parameters) , um die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="6c69e-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c69e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c69e-121">Request headers</span></span>

| <span data-ttu-id="6c69e-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c69e-122">Header</span></span>       | <span data-ttu-id="6c69e-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6c69e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c69e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c69e-124">Authorization</span></span>  | <span data-ttu-id="6c69e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6c69e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c69e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c69e-127">Content-Type</span></span>  | <span data-ttu-id="6c69e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6c69e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c69e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c69e-129">Request body</span></span>
<span data-ttu-id="6c69e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6c69e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c69e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c69e-131">Response</span></span>

<span data-ttu-id="6c69e-132">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [Shift](../resources/shift.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c69e-132">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c69e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c69e-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c69e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c69e-134">Request</span></span>

<span data-ttu-id="6c69e-135">Nachfolgend sehen Sie ein Beispiel für eine Anforderung, die alle **Shift** -Objekte mit einer freigegebenen Version und einer Entwurfsversion zwischen dem 11. März 2019.</span><span class="sxs-lookup"><span data-stu-id="6c69e-135">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```

#### <a name="response"></a><span data-ttu-id="6c69e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c69e-136">Response</span></span>

<span data-ttu-id="6c69e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c69e-137">The following is an example of the response.</span></span> 

><span data-ttu-id="6c69e-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6c69e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-list-shifts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
