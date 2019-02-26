---
title: Gruppe löschen – Microsoft Graph-API
description: Beschreibt die Delete-Methode der Group-Ressource (Entity) der Microsoft Graph-API (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 836f2c647fd9894a7d39bba80e5f15f3f11ef81f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255864"
---
# <a name="delete-group"></a><span data-ttu-id="ffadc-103">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="ffadc-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffadc-104">Löscht eine Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ffadc-104">Deletes a group.</span></span>  

<span data-ttu-id="ffadc-105">Nach dem Löschen werden Office 365-Gruppen in einen temporären Container verschoben und können innerhalb von 30 Tagen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="ffadc-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="ffadc-106">Nach diesem Zeitpunkt werden Sie dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="ffadc-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="ffadc-107">Weitere Informationen finden Sie unter [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ffadc-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="ffadc-108">Dies gilt nur für Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="ffadc-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffadc-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ffadc-109">Permissions</span></span>

<span data-ttu-id="ffadc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffadc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffadc-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffadc-112">Permission type</span></span>      | <span data-ttu-id="ffadc-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffadc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffadc-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffadc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ffadc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffadc-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffadc-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffadc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffadc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffadc-117">Not supported.</span></span>    |
|<span data-ttu-id="ffadc-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffadc-118">Application</span></span> | <span data-ttu-id="ffadc-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffadc-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffadc-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffadc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ffadc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffadc-121">Request headers</span></span>

| <span data-ttu-id="ffadc-122">Name</span><span class="sxs-lookup"><span data-stu-id="ffadc-122">Name</span></span>       | <span data-ttu-id="ffadc-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ffadc-123">Type</span></span> | <span data-ttu-id="ffadc-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffadc-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ffadc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffadc-125">Authorization</span></span>  | <span data-ttu-id="ffadc-126">string</span><span class="sxs-lookup"><span data-stu-id="ffadc-126">string</span></span>  | <span data-ttu-id="ffadc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffadc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffadc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffadc-129">Request body</span></span>

<span data-ttu-id="ffadc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ffadc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffadc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffadc-131">Response</span></span>

<span data-ttu-id="ffadc-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffadc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffadc-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffadc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffadc-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffadc-135">Request</span></span>

<span data-ttu-id="ffadc-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffadc-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="ffadc-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffadc-137">Response</span></span>

<span data-ttu-id="ffadc-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ffadc-138">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
