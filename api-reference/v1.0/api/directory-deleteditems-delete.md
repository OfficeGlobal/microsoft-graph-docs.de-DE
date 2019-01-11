---
title: Element endgültig löschen
description: Dauerhaftes Löschen eines Elements aus dem Ordner Gelöschte Elemente.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 00f44be1c89b35b81f3665d4bd568939ed309e22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805187"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="cccaa-103">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="cccaa-103">Permanently delete item</span></span>

<span data-ttu-id="cccaa-104">Dauerhaftes Löschen eines Elements aus dem Ordner [Gelöschte Elemente](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="cccaa-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="cccaa-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cccaa-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="cccaa-106">Sie können ein Element aus den gelöschten Elementen dauerhaft löschen.</span><span class="sxs-lookup"><span data-stu-id="cccaa-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="cccaa-107">Aber nachdem ein Element dauerhaft gelöscht wurde, **kann es nicht** wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="cccaa-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="cccaa-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cccaa-108">Permissions</span></span>
<span data-ttu-id="cccaa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cccaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="cccaa-111">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="cccaa-111">For users:</span></span>

|<span data-ttu-id="cccaa-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cccaa-112">Permission type</span></span>      | <span data-ttu-id="cccaa-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cccaa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cccaa-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cccaa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cccaa-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cccaa-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cccaa-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cccaa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cccaa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cccaa-117">Not supported.</span></span> |
|<span data-ttu-id="cccaa-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cccaa-118">Application</span></span> | <span data-ttu-id="cccaa-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cccaa-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="cccaa-120">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="cccaa-120">For groups:</span></span>

|<span data-ttu-id="cccaa-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cccaa-121">Permission type</span></span>      | <span data-ttu-id="cccaa-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cccaa-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cccaa-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cccaa-123">Delegated (work or school account)</span></span> | <span data-ttu-id="cccaa-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cccaa-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cccaa-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cccaa-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cccaa-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cccaa-126">Not supported.</span></span>    |
|<span data-ttu-id="cccaa-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cccaa-127">Application</span></span> | <span data-ttu-id="cccaa-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cccaa-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cccaa-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cccaa-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cccaa-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cccaa-130">Request headers</span></span>
| <span data-ttu-id="cccaa-131">Name</span><span class="sxs-lookup"><span data-stu-id="cccaa-131">Name</span></span>       | <span data-ttu-id="cccaa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cccaa-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cccaa-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cccaa-133">Authorization</span></span>  | <span data-ttu-id="cccaa-134">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="cccaa-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="cccaa-135">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cccaa-135">Accept</span></span>  | <span data-ttu-id="cccaa-136">application/json</span><span class="sxs-lookup"><span data-stu-id="cccaa-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cccaa-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cccaa-137">Request body</span></span>
<span data-ttu-id="cccaa-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cccaa-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cccaa-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="cccaa-139">Response</span></span>

<span data-ttu-id="cccaa-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cccaa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cccaa-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cccaa-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cccaa-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cccaa-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="cccaa-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="cccaa-144">Response</span></span>
<span data-ttu-id="cccaa-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cccaa-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
