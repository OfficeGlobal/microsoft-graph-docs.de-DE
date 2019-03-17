---
title: TimeOff löschen
description: Löscht eine timeOff-Instanz aus einem Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe3fdbe8445b11c9d1c0f176bccdc794e3a80480
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657490"
---
# <a name="delete-timeoff"></a><span data-ttu-id="e1b03-103">TimeOff löschen</span><span class="sxs-lookup"><span data-stu-id="e1b03-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b03-104">Löscht eine [timeOff](../resources/timeoff.md) -Instanz aus einem [Zeitplan](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="e1b03-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1b03-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1b03-105">Permissions</span></span>

<span data-ttu-id="e1b03-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1b03-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1b03-108">Permission type</span></span>      | <span data-ttu-id="e1b03-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1b03-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1b03-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1b03-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b03-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b03-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1b03-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1b03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b03-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1b03-113">Not supported.</span></span>    |
|<span data-ttu-id="e1b03-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1b03-114">Application</span></span> | <span data-ttu-id="e1b03-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1b03-115">Not supported.</span></span> |

> <span data-ttu-id="e1b03-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="e1b03-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e1b03-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="e1b03-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1b03-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1b03-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="e1b03-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1b03-119">Request headers</span></span>

| <span data-ttu-id="e1b03-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1b03-120">Header</span></span>       | <span data-ttu-id="e1b03-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e1b03-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1b03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1b03-122">Authorization</span></span>  | <span data-ttu-id="e1b03-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1b03-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1b03-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1b03-125">Content-Type</span></span>  | <span data-ttu-id="e1b03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b03-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1b03-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1b03-127">Request body</span></span>
<span data-ttu-id="e1b03-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1b03-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b03-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1b03-129">Response</span></span>

<span data-ttu-id="e1b03-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1b03-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b03-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1b03-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e1b03-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1b03-133">Request</span></span>

<span data-ttu-id="e1b03-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1b03-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="e1b03-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1b03-135">Response</span></span>

<span data-ttu-id="e1b03-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1b03-136">The following is an example of the response.</span></span> 

><span data-ttu-id="e1b03-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e1b03-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
