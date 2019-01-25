---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederherstellen einer vorherigen version
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7e430a3daf17ecf51500d258cc86a3dbbfcd108b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522455"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="1e35b-102">Frühere Version eines DriveItem wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="1e35b-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e35b-103">Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="1e35b-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="1e35b-104">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.</span><span class="sxs-lookup"><span data-stu-id="1e35b-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e35b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e35b-105">Permissions</span></span>

<span data-ttu-id="1e35b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e35b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e35b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e35b-108">Permission type</span></span>      | <span data-ttu-id="1e35b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e35b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e35b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e35b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e35b-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e35b-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e35b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e35b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e35b-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e35b-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e35b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e35b-114">Application</span></span> | <span data-ttu-id="1e35b-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e35b-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e35b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e35b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="1e35b-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e35b-117">Request body</span></span>

<span data-ttu-id="1e35b-118">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e35b-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="1e35b-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e35b-119">Example</span></span>

<span data-ttu-id="1e35b-120">In diesem Beispiel wird eine Version einer von `{item-id}` und `{version-id}` identifizierten Datei wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="1e35b-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="1e35b-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e35b-121">Response</span></span>

<span data-ttu-id="1e35b-122">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="1e35b-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
