---
author: chackman
ms.author: chackman
title: Nicht mehr folgen Laufwerk-Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 064ab2d5ad86df5341a0f2f5a46fe7c227ff35fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513109"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="03f81-102">Nicht mehr folgen Laufwerk-Element</span><span class="sxs-lookup"><span data-stu-id="03f81-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03f81-103">Nicht mehr folgen einer [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="03f81-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="03f81-104">**Hinweis:** Um ein Element zu befolgen, finden Sie unter [Artikel folgen](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="03f81-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03f81-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="03f81-105">Permissions</span></span>

<span data-ttu-id="03f81-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03f81-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03f81-108">Permission type</span></span>      | <span data-ttu-id="03f81-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03f81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03f81-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03f81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03f81-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f81-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="03f81-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03f81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03f81-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="03f81-113">Not supported.</span></span>    |
|<span data-ttu-id="03f81-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03f81-114">Application</span></span> | <span data-ttu-id="03f81-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f81-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03f81-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03f81-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="03f81-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03f81-117">Request body</span></span>

<span data-ttu-id="03f81-118">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="03f81-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="03f81-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="03f81-119">Response</span></span>

<span data-ttu-id="03f81-120">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="03f81-120">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="03f81-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03f81-121">Example</span></span>

<span data-ttu-id="03f81-122">In diesem Beispiel wird ein Element identifizierten unfollows `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="03f81-122">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
