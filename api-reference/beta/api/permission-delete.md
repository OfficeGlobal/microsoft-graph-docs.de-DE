---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Entfernen des Zugriffs auf ein Element
ms.openlocfilehash: 726818b14a694380e46bfd38280e4cba9effb67d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063307"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="6d441-102">Löschen einer Freigabeberechtigung aus einer Datei oder einem Ordner</span><span class="sxs-lookup"><span data-stu-id="6d441-102">Delete a sharing permission from a file or folder</span></span>

> <span data-ttu-id="6d441-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d441-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d441-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d441-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d441-105">Löschen Sie den Zugriff auf ein [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6d441-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="6d441-106">Es können nur **nicht** vererbte Berechtigungen gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="6d441-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="6d441-107">Die Eigenschaft **inheritedFrom** muss auf `null` gesetzt sein.</span><span class="sxs-lookup"><span data-stu-id="6d441-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d441-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d441-108">Permissions</span></span>
<span data-ttu-id="6d441-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d441-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d441-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d441-111">Permission type</span></span>      | <span data-ttu-id="6d441-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d441-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d441-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d441-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6d441-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d441-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d441-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d441-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d441-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d441-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d441-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d441-117">Application</span></span> | <span data-ttu-id="6d441-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d441-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d441-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d441-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6d441-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d441-120">Optional request headers</span></span>

| <span data-ttu-id="6d441-121">Name</span><span class="sxs-lookup"><span data-stu-id="6d441-121">Name</span></span>          | <span data-ttu-id="6d441-122">Typ</span><span class="sxs-lookup"><span data-stu-id="6d441-122">Type</span></span>   | <span data-ttu-id="6d441-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d441-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6d441-124">if-match</span><span class="sxs-lookup"><span data-stu-id="6d441-124">if-match</span></span>      | <span data-ttu-id="6d441-125">string</span><span class="sxs-lookup"><span data-stu-id="6d441-125">string</span></span> | <span data-ttu-id="6d441-126">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="6d441-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="6d441-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d441-127">Response</span></span>

<span data-ttu-id="6d441-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d441-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d441-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d441-129">Example</span></span>

<span data-ttu-id="6d441-130">In diesem Beispiel wird die als {perm-id} identifiziert Berechtigung des Elements {item-id} vom OneDrive des aktuellen Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="6d441-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="6d441-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d441-131">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="6d441-132">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="6d441-132">Remarks</span></span>

* <span data-ttu-id="6d441-133">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="6d441-133">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
