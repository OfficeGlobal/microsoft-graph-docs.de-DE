---
title: Frühere Version eines DriveItem wiederherstellen
description: Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her. Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.
localization_priority: Normal
ms.openlocfilehash: 0097d82bb9d317c0bee0392f21040f0963364183
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871610"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="3db9a-104">Frühere Version eines DriveItem wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="3db9a-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="3db9a-105">Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="3db9a-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="3db9a-106">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.</span><span class="sxs-lookup"><span data-stu-id="3db9a-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="3db9a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3db9a-107">Permissions</span></span>

<span data-ttu-id="3db9a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db9a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db9a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3db9a-110">Permission type</span></span>      | <span data-ttu-id="3db9a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3db9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db9a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3db9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3db9a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db9a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3db9a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3db9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db9a-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db9a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3db9a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3db9a-116">Application</span></span> | <span data-ttu-id="3db9a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db9a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db9a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db9a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="3db9a-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3db9a-119">Request body</span></span>

<span data-ttu-id="3db9a-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3db9a-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="3db9a-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3db9a-121">Example</span></span>

<span data-ttu-id="3db9a-122">In diesem Beispiel wird eine Version einer von `{item-id}` und `{version-id}` identifizierten Datei wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="3db9a-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="3db9a-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db9a-123">Response</span></span>

<span data-ttu-id="3db9a-124">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3db9a-124">If successful, the API call returns a `204 No Content`.</span></span>

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
