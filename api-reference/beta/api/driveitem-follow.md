---
author: chackman
ms.author: chackman
title: Führen Sie die Laufwerk-Element
localization_priority: Normal
ms.openlocfilehash: 5ba37773f552015b6c762b2b10d801b40670a03c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875033"
---
# <a name="follow-drive-item"></a><span data-ttu-id="22862-102">Führen Sie die Laufwerk-Element</span><span class="sxs-lookup"><span data-stu-id="22862-102">Follow drive item</span></span>

> <span data-ttu-id="22862-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22862-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22862-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22862-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22862-105">Führen Sie eine [DriveItem](../resources/driveitem.md)aus.</span><span class="sxs-lookup"><span data-stu-id="22862-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="22862-106">**Hinweis:** Wenn Sie ein Element nicht mehr folgen, finden Sie unter [Unfollow-Element](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="22862-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22862-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="22862-107">Permissions</span></span>

<span data-ttu-id="22862-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22862-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22862-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22862-110">Permission type</span></span>      | <span data-ttu-id="22862-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22862-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22862-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22862-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22862-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22862-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="22862-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22862-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22862-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22862-115">Not supported.</span></span>    |
|<span data-ttu-id="22862-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22862-116">Application</span></span> | <span data-ttu-id="22862-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22862-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22862-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22862-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="22862-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22862-119">Request body</span></span>

<span data-ttu-id="22862-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22862-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="22862-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="22862-121">Response</span></span>

<span data-ttu-id="22862-122">Diese Methode gibt eine [DriveItem](../resources/driveitem.md) für das Element gefolgt wird.</span><span class="sxs-lookup"><span data-stu-id="22862-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="22862-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22862-123">Example</span></span>

<span data-ttu-id="22862-124">In diesem Beispiel wird ein Element identifizierten folgt `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="22862-124">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!-- {
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow"
} -->

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
