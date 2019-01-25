---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Einchecken von Dateien
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ccb4a6dee07cd324a89a7f192b0fe1bb5aaa2e53
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529887"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="9dc8b-102">Einchecken-Änderungen für eine DriveItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="9dc8b-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dc8b-103">Checken Sie eine ausgecheckte DriveItem-Ressource ein, um die Version des Dokuments für andere verfügbar zu machen.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dc8b-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9dc8b-104">Permissions</span></span>

<span data-ttu-id="9dc8b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dc8b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9dc8b-107">Permission type</span></span>      | <span data-ttu-id="9dc8b-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9dc8b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dc8b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9dc8b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9dc8b-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc8b-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9dc8b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9dc8b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc8b-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc8b-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9dc8b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9dc8b-113">Application</span></span> | <span data-ttu-id="9dc8b-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc8b-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dc8b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dc8b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="9dc8b-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9dc8b-116">Request body</span></span>

<span data-ttu-id="9dc8b-117">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="9dc8b-118">Name</span><span class="sxs-lookup"><span data-stu-id="9dc8b-118">Name</span></span>    | <span data-ttu-id="9dc8b-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9dc8b-119">Value</span></span>  |                                                <span data-ttu-id="9dc8b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc8b-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9dc8b-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="9dc8b-121">checkInAs</span></span> | <span data-ttu-id="9dc8b-122">string</span><span class="sxs-lookup"><span data-stu-id="9dc8b-122">string</span></span> | <span data-ttu-id="9dc8b-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-123">Optional.</span></span> <span data-ttu-id="9dc8b-124">Der gewünschte Status des Dokuments nach Abschluss des Vorgangs Einchecken.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="9dc8b-125">Kann `published` oder nicht angegeben sein.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="9dc8b-126">Kommentar</span><span class="sxs-lookup"><span data-stu-id="9dc8b-126">comment</span></span>   | <span data-ttu-id="9dc8b-127">string</span><span class="sxs-lookup"><span data-stu-id="9dc8b-127">string</span></span> | <span data-ttu-id="9dc8b-128">Ein Eincheck-Kommentar, der mit der Version verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="9dc8b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9dc8b-129">Example</span></span>

<span data-ttu-id="9dc8b-130">In diesem Beispiel wird eine von `{item-id}` überprüfte Datei eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="9dc8b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dc8b-131">Response</span></span>

<span data-ttu-id="9dc8b-132">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="9dc8b-133">Hinweise</span><span class="sxs-lookup"><span data-stu-id="9dc8b-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
