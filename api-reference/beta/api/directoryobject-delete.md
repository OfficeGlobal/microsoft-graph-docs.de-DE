---
title: directoryObject löschen
description: directoryObject löschen
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63e9d4574c505158171c93fd7ac9dc51678c7d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507719"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="e8324-103">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="e8324-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8324-104">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="e8324-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8324-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8324-105">Permissions</span></span>
<span data-ttu-id="e8324-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8324-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8324-108">Permission type</span></span>      | <span data-ttu-id="e8324-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8324-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8324-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8324-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8324-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8324-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8324-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8324-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8324-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8324-113">Not supported.</span></span>    |
|<span data-ttu-id="e8324-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8324-114">Application</span></span> | <span data-ttu-id="e8324-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8324-115">Not supported.</span></span> |

<span data-ttu-id="e8324-116">**Hinweis:** Benutzer, Gruppen und Kontakte werden Typen von Directory-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e8324-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="e8324-117">Vorkommen, wenn Sie Benutzer löschen müssen, die folgende Berechtigung können und sollten verwendet werden: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8324-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="e8324-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8324-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e8324-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8324-119">Request headers</span></span>
| <span data-ttu-id="e8324-120">Name</span><span class="sxs-lookup"><span data-stu-id="e8324-120">Name</span></span>       | <span data-ttu-id="e8324-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e8324-121">Type</span></span> | <span data-ttu-id="e8324-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8324-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8324-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8324-123">Authorization</span></span>  | <span data-ttu-id="e8324-124">string</span><span class="sxs-lookup"><span data-stu-id="e8324-124">string</span></span>  | <span data-ttu-id="e8324-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e8324-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8324-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8324-127">Request body</span></span>
<span data-ttu-id="e8324-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8324-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8324-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8324-129">Response</span></span>

<span data-ttu-id="e8324-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8324-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8324-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8324-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8324-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8324-133">Request</span></span>
<span data-ttu-id="e8324-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8324-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="e8324-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8324-135">Response</span></span>
<span data-ttu-id="e8324-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8324-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
