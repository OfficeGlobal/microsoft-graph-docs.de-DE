---
title: directoryObject löschen
description: Löschen Sie DirectoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87ecefaac625153407bbc796870e540c3a4e83be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916215"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="27117-103">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="27117-103">Delete directoryObject</span></span>

> <span data-ttu-id="27117-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="27117-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27117-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27117-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27117-106">Löschen Sie DirectoryObject.</span><span class="sxs-lookup"><span data-stu-id="27117-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="27117-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="27117-107">Permissions</span></span>
<span data-ttu-id="27117-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27117-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27117-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27117-110">Permission type</span></span>      | <span data-ttu-id="27117-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27117-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27117-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27117-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27117-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27117-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27117-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27117-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27117-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27117-115">Not supported.</span></span>    |
|<span data-ttu-id="27117-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27117-116">Application</span></span> | <span data-ttu-id="27117-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27117-117">Not supported.</span></span> |

<span data-ttu-id="27117-118">**Hinweis:** Benutzer, Gruppen und Kontakte werden Typen von Directory-Objekt.</span><span class="sxs-lookup"><span data-stu-id="27117-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="27117-119">Vorkommen, wenn Sie Benutzer löschen müssen, die folgende Berechtigung können und sollten verwendet werden: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27117-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="27117-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27117-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="27117-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27117-121">Request headers</span></span>
| <span data-ttu-id="27117-122">Name</span><span class="sxs-lookup"><span data-stu-id="27117-122">Name</span></span>       | <span data-ttu-id="27117-123">Typ</span><span class="sxs-lookup"><span data-stu-id="27117-123">Type</span></span> | <span data-ttu-id="27117-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27117-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27117-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="27117-125">Authorization</span></span>  | <span data-ttu-id="27117-126">string</span><span class="sxs-lookup"><span data-stu-id="27117-126">string</span></span>  | <span data-ttu-id="27117-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="27117-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27117-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27117-129">Request body</span></span>
<span data-ttu-id="27117-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="27117-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27117-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="27117-131">Response</span></span>

<span data-ttu-id="27117-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27117-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27117-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27117-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27117-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27117-135">Request</span></span>
<span data-ttu-id="27117-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27117-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="27117-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="27117-137">Response</span></span>
<span data-ttu-id="27117-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="27117-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
