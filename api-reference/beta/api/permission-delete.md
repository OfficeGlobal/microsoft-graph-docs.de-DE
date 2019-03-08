---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Entfernen des Zugriffs auf ein Element
localization_priority: Normal
ms.openlocfilehash: 3cc4f6a151d2990c5180e02888484e1260704f04
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480558"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="4be00-102">Eine Freigabeberechtigung aus einer Datei oder einem Ordner löschen</span><span class="sxs-lookup"><span data-stu-id="4be00-102">Delete a sharing permission from a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be00-103">Löschen Sie den Zugriff auf ein [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4be00-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="4be00-104">Es können nur **nicht** vererbte Berechtigungen gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="4be00-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="4be00-105">Die Eigenschaft **inheritedFrom** muss auf `null` gesetzt sein.</span><span class="sxs-lookup"><span data-stu-id="4be00-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be00-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4be00-106">Permissions</span></span>
<span data-ttu-id="4be00-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be00-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4be00-109">Permission type</span></span>      | <span data-ttu-id="4be00-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4be00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be00-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4be00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4be00-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be00-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4be00-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4be00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be00-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be00-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4be00-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4be00-115">Application</span></span> | <span data-ttu-id="4be00-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be00-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be00-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4be00-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4be00-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4be00-118">Optional request headers</span></span>

| <span data-ttu-id="4be00-119">Name</span><span class="sxs-lookup"><span data-stu-id="4be00-119">Name</span></span>          | <span data-ttu-id="4be00-120">Typ</span><span class="sxs-lookup"><span data-stu-id="4be00-120">Type</span></span>   | <span data-ttu-id="4be00-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4be00-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4be00-122">if-match</span><span class="sxs-lookup"><span data-stu-id="4be00-122">if-match</span></span>      | <span data-ttu-id="4be00-123">string</span><span class="sxs-lookup"><span data-stu-id="4be00-123">string</span></span> | <span data-ttu-id="4be00-124">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="4be00-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="4be00-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="4be00-125">Response</span></span>

<span data-ttu-id="4be00-126">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4be00-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4be00-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4be00-127">Example</span></span>

<span data-ttu-id="4be00-128">In diesem Beispiel wird die als {perm-id} identifiziert Berechtigung des Elements {item-id} vom OneDrive des aktuellen Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="4be00-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="4be00-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4be00-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="4be00-130">HinwBemerkungeneise</span><span class="sxs-lookup"><span data-stu-id="4be00-130">Remarks</span></span>

* <span data-ttu-id="4be00-131">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="4be00-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
    "Error: /api-reference/beta/api/permission-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
