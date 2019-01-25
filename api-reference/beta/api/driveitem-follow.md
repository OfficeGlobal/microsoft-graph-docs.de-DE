---
author: chackman
ms.author: chackman
title: Führen Sie die Laufwerk-Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0c8835593ed7203cc6239485f1dcd4f17f24fe7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518338"
---
# <a name="follow-drive-item"></a><span data-ttu-id="29dcd-102">Führen Sie die Laufwerk-Element</span><span class="sxs-lookup"><span data-stu-id="29dcd-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29dcd-103">Führen Sie eine [DriveItem](../resources/driveitem.md)aus.</span><span class="sxs-lookup"><span data-stu-id="29dcd-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="29dcd-104">**Hinweis:** Wenn Sie ein Element nicht mehr folgen, finden Sie unter [Unfollow-Element](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="29dcd-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29dcd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29dcd-105">Permissions</span></span>

<span data-ttu-id="29dcd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29dcd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29dcd-108">Permission type</span></span>      | <span data-ttu-id="29dcd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29dcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29dcd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29dcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29dcd-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29dcd-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="29dcd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29dcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29dcd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29dcd-113">Not supported.</span></span>    |
|<span data-ttu-id="29dcd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29dcd-114">Application</span></span> | <span data-ttu-id="29dcd-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29dcd-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29dcd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29dcd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="29dcd-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29dcd-117">Request body</span></span>

<span data-ttu-id="29dcd-118">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29dcd-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="29dcd-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="29dcd-119">Response</span></span>

<span data-ttu-id="29dcd-120">Diese Methode gibt eine [DriveItem](../resources/driveitem.md) für das Element gefolgt wird.</span><span class="sxs-lookup"><span data-stu-id="29dcd-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="29dcd-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29dcd-121">Example</span></span>

<span data-ttu-id="29dcd-122">In diesem Beispiel wird ein Element identifizierten folgt `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="29dcd-122">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
