---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Auschecken von Dateien
localization_priority: Normal
ms.openlocfilehash: 4201f9a075947182cdcd2b69b222896e3c60f93d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870000"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="376f5-102">DriveItem-Ressource auschecken</span><span class="sxs-lookup"><span data-stu-id="376f5-102">Check-out a DriveItem resource</span></span>

> <span data-ttu-id="376f5-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="376f5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="376f5-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="376f5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="376f5-105">Checken Sie eine DriveItem-Ressource aus, damit andere Benutzer das Dokument nicht bearbeiten können und Ihre Änderungen erst sichtbar werden, wenn das Dokument [eingecheckt](driveitem-checkin.md) wird.</span><span class="sxs-lookup"><span data-stu-id="376f5-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="376f5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="376f5-106">Permissions</span></span>

<span data-ttu-id="376f5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376f5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="376f5-109">Permission type</span></span>      | <span data-ttu-id="376f5-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="376f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="376f5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="376f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="376f5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376f5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="376f5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="376f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="376f5-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376f5-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="376f5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="376f5-115">Application</span></span> | <span data-ttu-id="376f5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376f5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="376f5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="376f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="376f5-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="376f5-118">Request body</span></span>

<span data-ttu-id="376f5-119">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="376f5-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="376f5-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="376f5-120">Example</span></span>

<span data-ttu-id="376f5-121">In diesem Beispiel wird eine von `{item-id}` überprüfte Datei ausgecheckt.</span><span class="sxs-lookup"><span data-stu-id="376f5-121">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="376f5-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="376f5-122">Response</span></span>

<span data-ttu-id="376f5-123">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="376f5-123">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="376f5-124">Hinweise</span><span class="sxs-lookup"><span data-stu-id="376f5-124">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
