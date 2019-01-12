---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Einchecken von Dateien
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fb62dc05c60e26a6d1d6683913eeec0403d1c41c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950809"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="35bb3-102">Einchecken-Änderungen für eine DriveItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="35bb3-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="35bb3-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35bb3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35bb3-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35bb3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35bb3-105">Checken Sie eine ausgecheckte DriveItem-Ressource ein, um die Version des Dokuments für andere verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="35bb3-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="35bb3-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="35bb3-106">Permissions</span></span>

<span data-ttu-id="35bb3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35bb3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35bb3-109">Permission type</span></span>      | <span data-ttu-id="35bb3-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35bb3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35bb3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35bb3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35bb3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35bb3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="35bb3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35bb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35bb3-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35bb3-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="35bb3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35bb3-115">Application</span></span> | <span data-ttu-id="35bb3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35bb3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35bb3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35bb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="35bb3-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35bb3-118">Request body</span></span>

<span data-ttu-id="35bb3-119">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="35bb3-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="35bb3-120">Name</span><span class="sxs-lookup"><span data-stu-id="35bb3-120">Name</span></span>    | <span data-ttu-id="35bb3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="35bb3-121">Value</span></span>  |                                                <span data-ttu-id="35bb3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35bb3-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="35bb3-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="35bb3-123">checkInAs</span></span> | <span data-ttu-id="35bb3-124">string</span><span class="sxs-lookup"><span data-stu-id="35bb3-124">string</span></span> | <span data-ttu-id="35bb3-125">Optional.</span><span class="sxs-lookup"><span data-stu-id="35bb3-125">Optional.</span></span> <span data-ttu-id="35bb3-126">Der gewünschte Status des Dokuments nach Abschluss des Vorgangs Einchecken.</span><span class="sxs-lookup"><span data-stu-id="35bb3-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="35bb3-127">Kann `published` oder nicht angegeben sein.</span><span class="sxs-lookup"><span data-stu-id="35bb3-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="35bb3-128">Kommentar</span><span class="sxs-lookup"><span data-stu-id="35bb3-128">comment</span></span>   | <span data-ttu-id="35bb3-129">string</span><span class="sxs-lookup"><span data-stu-id="35bb3-129">string</span></span> | <span data-ttu-id="35bb3-130">Ein Eincheck-Kommentar, der mit der Version verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="35bb3-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="35bb3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35bb3-131">Example</span></span>

<span data-ttu-id="35bb3-132">In diesem Beispiel wird eine von `{item-id}` überprüfte Datei eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="35bb3-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="35bb3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="35bb3-133">Response</span></span>

<span data-ttu-id="35bb3-134">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="35bb3-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="35bb3-135">Hinweise</span><span class="sxs-lookup"><span data-stu-id="35bb3-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
