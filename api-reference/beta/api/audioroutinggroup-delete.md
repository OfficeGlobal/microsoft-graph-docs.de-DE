---
title: Audio Routinggruppe löschen
description: Löschen der angegebenen audio Routinggruppe.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0c0e5c0cd58c867f7c69a3ac5d4f99a11af223ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511443"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="e04d0-103">Audio Routinggruppe löschen</span><span class="sxs-lookup"><span data-stu-id="e04d0-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e04d0-104">Löschen der angegebenen [AudioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="e04d0-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e04d0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e04d0-105">Permissions</span></span>
<span data-ttu-id="e04d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e04d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e04d0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e04d0-108">Permission type</span></span> | <span data-ttu-id="e04d0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e04d0-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="e04d0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e04d0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e04d0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e04d0-111">Not Supported</span></span>        |
| <span data-ttu-id="e04d0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e04d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e04d0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e04d0-113">Not Supported</span></span>        |
| <span data-ttu-id="e04d0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e04d0-114">Application</span></span>     | <span data-ttu-id="e04d0-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="e04d0-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e04d0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e04d0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e04d0-117">Request headers</span></span>
| <span data-ttu-id="e04d0-118">Name</span><span class="sxs-lookup"><span data-stu-id="e04d0-118">Name</span></span>          | <span data-ttu-id="e04d0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e04d0-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e04d0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e04d0-120">Authorization</span></span> | <span data-ttu-id="e04d0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e04d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e04d0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e04d0-123">Request body</span></span>
<span data-ttu-id="e04d0-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e04d0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e04d0-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04d0-125">Response</span></span>
<span data-ttu-id="e04d0-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e04d0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e04d0-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e04d0-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e04d0-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e04d0-129">Request</span></span>
<span data-ttu-id="e04d0-130">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="e04d0-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="e04d0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e04d0-131">Response</span></span>

> <span data-ttu-id="e04d0-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e04d0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
