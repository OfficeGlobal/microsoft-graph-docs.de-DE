---
title: Gruppe löschen
description: Löscht eine Gruppe.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 349900cffa4b0df1763e1ed8b8213ce81ec27351
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529964"
---
# <a name="delete-group"></a><span data-ttu-id="c13df-103">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="c13df-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13df-104">Löscht eine Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c13df-104">Deletes a group.</span></span>

<span data-ttu-id="c13df-105">Wenn eine Gruppe gelöscht wird, wird das Element [Gelöschte Elemente](../resources/directory.md)hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c13df-105">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="c13df-106">Die Gruppe bleibt in gelöschte Elemente für bis zu 30 Tage.</span><span class="sxs-lookup"><span data-stu-id="c13df-106">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="c13df-107">Eine Gruppe kann von gelöschten Objekten innerhalb der letzten 30 Tage vollständig wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c13df-107">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="c13df-108">Nach 30 Tagen werden gelöschte Elemente dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="c13df-108">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="c13df-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c13df-109">Permissions</span></span>
<span data-ttu-id="c13df-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c13df-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c13df-112">Permission type</span></span>      | <span data-ttu-id="c13df-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c13df-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c13df-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c13df-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c13df-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13df-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c13df-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c13df-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13df-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c13df-117">Not supported.</span></span>    |
|<span data-ttu-id="c13df-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c13df-118">Application</span></span> | <span data-ttu-id="c13df-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13df-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c13df-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c13df-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c13df-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c13df-121">Request headers</span></span>
| <span data-ttu-id="c13df-122">Name</span><span class="sxs-lookup"><span data-stu-id="c13df-122">Name</span></span>       | <span data-ttu-id="c13df-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c13df-123">Type</span></span> | <span data-ttu-id="c13df-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c13df-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c13df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c13df-125">Authorization</span></span>  | <span data-ttu-id="c13df-126">string</span><span class="sxs-lookup"><span data-stu-id="c13df-126">string</span></span>  | <span data-ttu-id="c13df-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c13df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c13df-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c13df-129">Request body</span></span>
<span data-ttu-id="c13df-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c13df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c13df-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c13df-131">Response</span></span>
<span data-ttu-id="c13df-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c13df-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c13df-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c13df-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c13df-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c13df-135">Request</span></span>
<span data-ttu-id="c13df-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c13df-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="c13df-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c13df-137">Response</span></span>
<span data-ttu-id="c13df-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c13df-138">The following is an example of the response.</span></span> 
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
