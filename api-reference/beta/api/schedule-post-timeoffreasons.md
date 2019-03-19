---
title: TimeOffReason erstellen
description: Erstellen Sie eine neue timeOffReason.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 33cf5e7c0cb04c6573145f542e9096b974187912
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657784"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="a63c5-103">TimeOffReason erstellen</span><span class="sxs-lookup"><span data-stu-id="a63c5-103">Create timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a63c5-104">Erstellen Sie eine neue [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="a63c5-104">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a63c5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a63c5-105">Permissions</span></span>

<span data-ttu-id="a63c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a63c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a63c5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a63c5-108">Permission type</span></span>      | <span data-ttu-id="a63c5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a63c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a63c5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a63c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a63c5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a63c5-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a63c5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a63c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a63c5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a63c5-113">Not supported.</span></span>    |
|<span data-ttu-id="a63c5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a63c5-114">Application</span></span> | <span data-ttu-id="a63c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a63c5-115">Not supported.</span></span> |

> <span data-ttu-id="a63c5-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a63c5-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a63c5-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="a63c5-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a63c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a63c5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="a63c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a63c5-119">Request headers</span></span>

| <span data-ttu-id="a63c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a63c5-120">Header</span></span>       | <span data-ttu-id="a63c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a63c5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a63c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a63c5-122">Authorization</span></span>  | <span data-ttu-id="a63c5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a63c5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a63c5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a63c5-125">Content-Type</span></span>  | <span data-ttu-id="a63c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a63c5-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="a63c5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a63c5-127">Response</span></span>

<span data-ttu-id="a63c5-128">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [timeOffReason](../resources/timeoffreason.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a63c5-128">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a63c5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a63c5-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a63c5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a63c5-130">Request</span></span>

<span data-ttu-id="a63c5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a63c5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```

#### <a name="response"></a><span data-ttu-id="a63c5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a63c5-132">Response</span></span>

<span data-ttu-id="a63c5-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a63c5-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a63c5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a63c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-timeoffreasons.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->