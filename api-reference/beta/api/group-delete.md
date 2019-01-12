---
title: Gruppe löschen
description: Löscht eine Gruppe.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 75b5d03cb5bce93966efc1495fd4284060580189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916453"
---
# <a name="delete-group"></a><span data-ttu-id="47cda-103">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="47cda-103">Delete group</span></span>

> <span data-ttu-id="47cda-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="47cda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47cda-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47cda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47cda-106">Löscht eine Gruppe.</span><span class="sxs-lookup"><span data-stu-id="47cda-106">Deletes a group.</span></span>

<span data-ttu-id="47cda-107">Wenn eine Gruppe gelöscht wird, wird das Element [Gelöschte Elemente](../resources/directory.md)hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="47cda-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="47cda-108">Die Gruppe bleibt in gelöschte Elemente für bis zu 30 Tage.</span><span class="sxs-lookup"><span data-stu-id="47cda-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="47cda-109">Eine Gruppe kann von gelöschten Objekten innerhalb der letzten 30 Tage vollständig wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="47cda-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="47cda-110">Nach 30 Tagen werden gelöschte Elemente dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="47cda-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="47cda-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="47cda-111">Permissions</span></span>
<span data-ttu-id="47cda-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47cda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47cda-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47cda-114">Permission type</span></span>      | <span data-ttu-id="47cda-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47cda-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47cda-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47cda-116">Delegated (work or school account)</span></span> | <span data-ttu-id="47cda-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47cda-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47cda-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47cda-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47cda-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47cda-119">Not supported.</span></span>    |
|<span data-ttu-id="47cda-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47cda-120">Application</span></span> | <span data-ttu-id="47cda-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47cda-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47cda-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47cda-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47cda-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47cda-123">Request headers</span></span>
| <span data-ttu-id="47cda-124">Name</span><span class="sxs-lookup"><span data-stu-id="47cda-124">Name</span></span>       | <span data-ttu-id="47cda-125">Typ</span><span class="sxs-lookup"><span data-stu-id="47cda-125">Type</span></span> | <span data-ttu-id="47cda-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47cda-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47cda-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="47cda-127">Authorization</span></span>  | <span data-ttu-id="47cda-128">string</span><span class="sxs-lookup"><span data-stu-id="47cda-128">string</span></span>  | <span data-ttu-id="47cda-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="47cda-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47cda-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47cda-131">Request body</span></span>
<span data-ttu-id="47cda-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47cda-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47cda-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="47cda-133">Response</span></span>
<span data-ttu-id="47cda-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47cda-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47cda-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47cda-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="47cda-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47cda-137">Request</span></span>
<span data-ttu-id="47cda-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47cda-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="47cda-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="47cda-139">Response</span></span>
<span data-ttu-id="47cda-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="47cda-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
