---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederherstellen einer vorherigen version
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9f8492b3a6e4b01b61288b235cc0dfa19ffd78d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946077"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="02154-102">Frühere Version eines DriveItem wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="02154-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="02154-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02154-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02154-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02154-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02154-105">Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="02154-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="02154-106">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.</span><span class="sxs-lookup"><span data-stu-id="02154-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="02154-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02154-107">Permissions</span></span>

<span data-ttu-id="02154-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02154-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02154-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02154-110">Permission type</span></span>      | <span data-ttu-id="02154-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02154-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02154-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02154-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02154-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02154-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="02154-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02154-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02154-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02154-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="02154-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02154-116">Application</span></span> | <span data-ttu-id="02154-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02154-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02154-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02154-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="02154-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02154-119">Request body</span></span>

<span data-ttu-id="02154-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02154-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="02154-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02154-121">Example</span></span>

<span data-ttu-id="02154-122">In diesem Beispiel wird eine Version einer von `{item-id}` und `{version-id}` identifizierten Datei wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="02154-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="02154-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="02154-123">Response</span></span>

<span data-ttu-id="02154-124">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="02154-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
