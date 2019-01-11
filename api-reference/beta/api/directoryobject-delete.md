---
title: directoryObject löschen
description: Löschen Sie DirectoryObject.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: e291004f13eaf6d0f24750002c8068d3e97b3052
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865201"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="87cfd-103">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="87cfd-103">Delete directoryObject</span></span>

> <span data-ttu-id="87cfd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87cfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87cfd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87cfd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87cfd-106">Löschen Sie DirectoryObject.</span><span class="sxs-lookup"><span data-stu-id="87cfd-106">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="87cfd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87cfd-107">Permissions</span></span>
<span data-ttu-id="87cfd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87cfd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87cfd-110">Permission type</span></span>      | <span data-ttu-id="87cfd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87cfd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87cfd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87cfd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87cfd-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87cfd-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87cfd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87cfd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87cfd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87cfd-115">Not supported.</span></span>    |
|<span data-ttu-id="87cfd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87cfd-116">Application</span></span> | <span data-ttu-id="87cfd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87cfd-117">Not supported.</span></span> |

<span data-ttu-id="87cfd-118">**Hinweis:** Benutzer, Gruppen und Kontakte werden Typen von Directory-Objekt.</span><span class="sxs-lookup"><span data-stu-id="87cfd-118">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="87cfd-119">Vorkommen, wenn Sie Benutzer löschen müssen, die folgende Berechtigung können und sollten verwendet werden: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87cfd-119">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="87cfd-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87cfd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="87cfd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87cfd-121">Request headers</span></span>
| <span data-ttu-id="87cfd-122">Name</span><span class="sxs-lookup"><span data-stu-id="87cfd-122">Name</span></span>       | <span data-ttu-id="87cfd-123">Typ</span><span class="sxs-lookup"><span data-stu-id="87cfd-123">Type</span></span> | <span data-ttu-id="87cfd-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87cfd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87cfd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87cfd-125">Authorization</span></span>  | <span data-ttu-id="87cfd-126">string</span><span class="sxs-lookup"><span data-stu-id="87cfd-126">string</span></span>  | <span data-ttu-id="87cfd-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87cfd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87cfd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87cfd-129">Request body</span></span>
<span data-ttu-id="87cfd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87cfd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87cfd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="87cfd-131">Response</span></span>

<span data-ttu-id="87cfd-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87cfd-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87cfd-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87cfd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87cfd-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87cfd-135">Request</span></span>
<span data-ttu-id="87cfd-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87cfd-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="87cfd-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="87cfd-137">Response</span></span>
<span data-ttu-id="87cfd-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87cfd-138">Here is an example of the response.</span></span> 
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
