---
title: TimeOffReason löschen
description: Kennzeichnen einer timeOffReason als inaktiv, indem Sie die IsActive-Eigenschaft festlegen
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: adf5c7b25f2a0fada834f5d865958cba89673df3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657679"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="48a83-103">TimeOffReason löschen</span><span class="sxs-lookup"><span data-stu-id="48a83-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a83-104">Markieren Sie eine [timeOffReason](../resources/timeoffreason.md) als inaktiv, indem Sie die IsActive-Eigenschaft festlegen. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="48a83-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="48a83-105">Mit dieser Methode wird die angegebene [timeOffReason](../resources/timeoffreason.md) -Instanz nicht entfernt.</span><span class="sxs-lookup"><span data-stu-id="48a83-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="48a83-106">[timeOffItem](../resources/timeoffitem.md) -Instanzen, denen dieser Grund zugewiesen wurde, bleiben diesem Grund zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="48a83-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="48a83-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48a83-107">Permissions</span></span>

<span data-ttu-id="48a83-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a83-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48a83-110">Permission type</span></span>      | <span data-ttu-id="48a83-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48a83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48a83-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48a83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48a83-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a83-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48a83-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48a83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a83-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48a83-115">Not supported.</span></span>    |
|<span data-ttu-id="48a83-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48a83-116">Application</span></span> | <span data-ttu-id="48a83-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48a83-117">Not supported.</span></span> |

> <span data-ttu-id="48a83-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="48a83-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="48a83-119">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="48a83-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="48a83-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48a83-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="48a83-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48a83-121">Request headers</span></span>

| <span data-ttu-id="48a83-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48a83-122">Header</span></span>       | <span data-ttu-id="48a83-123">Wert</span><span class="sxs-lookup"><span data-stu-id="48a83-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48a83-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="48a83-124">Authorization</span></span>  | <span data-ttu-id="48a83-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48a83-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48a83-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48a83-127">Content-Type</span></span>  | <span data-ttu-id="48a83-128">application/json</span><span class="sxs-lookup"><span data-stu-id="48a83-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48a83-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48a83-129">Request body</span></span>
<span data-ttu-id="48a83-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="48a83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48a83-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="48a83-131">Response</span></span>

<span data-ttu-id="48a83-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48a83-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48a83-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48a83-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48a83-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48a83-135">Request</span></span>

<span data-ttu-id="48a83-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48a83-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="48a83-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="48a83-137">Response</span></span>

<span data-ttu-id="48a83-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48a83-138">The following is an example of the response.</span></span> 

><span data-ttu-id="48a83-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="48a83-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
