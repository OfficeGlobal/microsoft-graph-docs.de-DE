---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AusChecken von Dateien
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bd69a02a3c243a86d7f9d05b54eb3fac00eeee88
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481293"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="29b9e-102">DriveItem-Ressource auschecken</span><span class="sxs-lookup"><span data-stu-id="29b9e-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b9e-103">Checken Sie eine DriveItem-Ressource aus, damit andere Benutzer das Dokument nicht bearbeiten können und Ihre Änderungen erst sichtbar werden, wenn das Dokument [eingecheckt](driveitem-checkin.md) wird.</span><span class="sxs-lookup"><span data-stu-id="29b9e-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29b9e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29b9e-104">Permissions</span></span>

<span data-ttu-id="29b9e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b9e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29b9e-107">Permission type</span></span>      | <span data-ttu-id="29b9e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29b9e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29b9e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29b9e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="29b9e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b9e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="29b9e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29b9e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29b9e-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b9e-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="29b9e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29b9e-113">Application</span></span> | <span data-ttu-id="29b9e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b9e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29b9e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29b9e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="29b9e-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29b9e-116">Request body</span></span>

<span data-ttu-id="29b9e-117">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29b9e-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="29b9e-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29b9e-118">Example</span></span>

<span data-ttu-id="29b9e-119">In diesem Beispiel wird eine von `{item-id}` überprüfte Datei ausgecheckt.</span><span class="sxs-lookup"><span data-stu-id="29b9e-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="29b9e-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="29b9e-120">Response</span></span>

<span data-ttu-id="29b9e-121">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="29b9e-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="29b9e-122">Hinweise</span><span class="sxs-lookup"><span data-stu-id="29b9e-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
