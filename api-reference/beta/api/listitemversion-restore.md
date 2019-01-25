---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederherstellen einer früheren Version eines SharePoint-Listenelements
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ef3b5848b6a6f60bf0515f914e87383e0a6f66bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511555"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="252bb-102">Frühere Version eines SharePoint-Listenelements wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="252bb-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="252bb-103">Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="252bb-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="252bb-104">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="252bb-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="252bb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="252bb-105">Permissions</span></span>

<span data-ttu-id="252bb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="252bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="252bb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="252bb-108">Permission type</span></span>             |         <span data-ttu-id="252bb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="252bb-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="252bb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="252bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="252bb-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="252bb-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="252bb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="252bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="252bb-113">N/V</span><span class="sxs-lookup"><span data-stu-id="252bb-113">n/a</span></span>                                                          |
| <span data-ttu-id="252bb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="252bb-114">Application</span></span>                            | <span data-ttu-id="252bb-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="252bb-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="252bb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="252bb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="252bb-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="252bb-117">Request body</span></span>

<span data-ttu-id="252bb-118">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="252bb-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="252bb-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="252bb-119">Example</span></span>

<span data-ttu-id="252bb-120">In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="252bb-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="252bb-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="252bb-121">Response</span></span>

<span data-ttu-id="252bb-122">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="252bb-122">If successful, the API call returns a `204 No content`.</span></span>

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
