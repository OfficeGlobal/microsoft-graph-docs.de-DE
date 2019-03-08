---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Wiederherstellen einer früheren Version eines SharePoint-Listenelements
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20cf0460aa679fc40a4bb11d0887bc4946ddcd74
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482084"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="5829d-102">Frühere Version eines SharePoint-Listenelements wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="5829d-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5829d-103">Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="5829d-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="5829d-104">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="5829d-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="5829d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5829d-105">Permissions</span></span>

<span data-ttu-id="5829d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5829d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="5829d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5829d-108">Permission type</span></span>             |         <span data-ttu-id="5829d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5829d-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5829d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5829d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5829d-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5829d-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="5829d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5829d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5829d-113">N/V</span><span class="sxs-lookup"><span data-stu-id="5829d-113">n/a</span></span>                                                          |
| <span data-ttu-id="5829d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5829d-114">Application</span></span>                            | <span data-ttu-id="5829d-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5829d-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5829d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5829d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="5829d-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5829d-117">Request body</span></span>

<span data-ttu-id="5829d-118">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5829d-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="5829d-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5829d-119">Example</span></span>

<span data-ttu-id="5829d-120">In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="5829d-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="5829d-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="5829d-121">Response</span></span>

<span data-ttu-id="5829d-122">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="5829d-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
