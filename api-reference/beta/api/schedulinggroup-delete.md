---
title: Planungsgroup löschen
description: Kennzeichnen Sie eine schedulinggroup als inaktiv, indem Sie Ihre IsActive-Eigenschaft festlegen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb29270cdf246924f0c6a9293611bec82dac5cc3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657714"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="8a708-103">Planungsgroup löschen</span><span class="sxs-lookup"><span data-stu-id="8a708-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a708-104">Markieren Sie [](../resources/schedulinggroup.md) eine schedulinggroup als inaktiv, indem Sie Ihre IsActive-Eigenschaft festlegen. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="8a708-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="8a708-105">Diese Methode entfernt die schedulinggroup [](../resources/schedulinggroup.md) nicht aus dem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="8a708-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="8a708-106">Vorhandene [Shift](../resources/shift.md) -Instanzen, die der Planungsgruppe zugewiesen sind, bleiben Teil der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="8a708-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a708-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a708-107">Permissions</span></span>

<span data-ttu-id="8a708-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a708-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a708-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a708-110">Permission type</span></span>      | <span data-ttu-id="8a708-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a708-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a708-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a708-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a708-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a708-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a708-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a708-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a708-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a708-115">Not supported.</span></span>    |
|<span data-ttu-id="8a708-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a708-116">Application</span></span> | <span data-ttu-id="8a708-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a708-117">Not supported.</span></span> |

> <span data-ttu-id="8a708-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8a708-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8a708-119">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="8a708-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a708-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a708-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="8a708-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a708-121">Request headers</span></span>

| <span data-ttu-id="8a708-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8a708-122">Header</span></span>       | <span data-ttu-id="8a708-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8a708-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a708-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a708-124">Authorization</span></span>  | <span data-ttu-id="8a708-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a708-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a708-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a708-127">Content-Type</span></span>  | <span data-ttu-id="8a708-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8a708-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a708-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a708-129">Request body</span></span>
<span data-ttu-id="8a708-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8a708-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a708-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a708-131">Response</span></span>

<span data-ttu-id="8a708-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a708-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a708-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a708-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a708-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a708-135">Request</span></span>

<span data-ttu-id="8a708-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a708-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="8a708-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a708-137">Response</span></span>

<span data-ttu-id="8a708-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8a708-138">The following is an example of the response.</span></span> 

><span data-ttu-id="8a708-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8a708-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-delete-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
