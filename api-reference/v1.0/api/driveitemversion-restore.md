---
title: Frühere Version eines DriveItem wiederherstellen
description: Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her. Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bfc4513b958d74aae40e7108f2c0b59b570e5c6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990355"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="e8e8d-104">Frühere Version eines DriveItem wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="e8e8d-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="e8e8d-105">Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="e8e8d-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="e8e8d-106">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.</span><span class="sxs-lookup"><span data-stu-id="e8e8d-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e8d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8e8d-107">Permissions</span></span>

<span data-ttu-id="e8e8d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e8d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8e8d-110">Permission type</span></span>      | <span data-ttu-id="e8e8d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8e8d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8e8d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8e8d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e8d-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e8d-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8e8d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8e8d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e8d-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e8d-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8e8d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8e8d-116">Application</span></span> | <span data-ttu-id="e8e8d-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e8d-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8e8d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8e8d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="e8e8d-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8e8d-119">Request body</span></span>

<span data-ttu-id="e8e8d-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8e8d-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="e8e8d-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8e8d-121">Example</span></span>

<span data-ttu-id="e8e8d-122">In diesem Beispiel wird eine Version einer von `{item-id}` und `{version-id}` identifizierten Datei wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="e8e8d-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="e8e8d-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8e8d-123">Response</span></span>

<span data-ttu-id="e8e8d-124">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e8e8d-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
