---
author: chackman
ms.author: chackman
title: Nicht mehr folgen Laufwerk-Element
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a42f740b3ea6f706529a5353e9cbb846bb7a4e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945951"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="df680-102">Nicht mehr folgen Laufwerk-Element</span><span class="sxs-lookup"><span data-stu-id="df680-102">Unfollow drive item</span></span>

> <span data-ttu-id="df680-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df680-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df680-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df680-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df680-105">Nicht mehr folgen einer [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="df680-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="df680-106">**Hinweis:** Um ein Element zu befolgen, finden Sie unter [Artikel folgen](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="df680-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df680-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="df680-107">Permissions</span></span>

<span data-ttu-id="df680-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df680-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df680-110">Permission type</span></span>      | <span data-ttu-id="df680-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df680-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df680-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df680-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df680-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df680-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="df680-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df680-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df680-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df680-115">Not supported.</span></span>    |
|<span data-ttu-id="df680-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df680-116">Application</span></span> | <span data-ttu-id="df680-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df680-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df680-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df680-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="df680-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df680-119">Request body</span></span>

<span data-ttu-id="df680-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df680-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="df680-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="df680-121">Response</span></span>

<span data-ttu-id="df680-122">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="df680-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="df680-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df680-123">Example</span></span>

<span data-ttu-id="df680-124">In diesem Beispiel wird ein Element identifizierten unfollows `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="df680-124">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!-- {
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow"
} -->
