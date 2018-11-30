---
title: directoryObject löschen
description: Mit dieser API können Sie eine Ressource des Typs „directoryObject“ löschen.
ms.openlocfilehash: 2ecd16163a7241b34adc74ebc1aa8c11406cb800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019393"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="c2078-103">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="c2078-103">Delete directoryObject</span></span>

<span data-ttu-id="c2078-104">Mit dieser API können Sie eine Ressource des Typs „directoryObject“ löschen.</span><span class="sxs-lookup"><span data-stu-id="c2078-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2078-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2078-105">Permissions</span></span>
<span data-ttu-id="c2078-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c2078-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2078-108">Permission type</span></span>      | <span data-ttu-id="c2078-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2078-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2078-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2078-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2078-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2078-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2078-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2078-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2078-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2078-113">Not supported.</span></span>    |
|<span data-ttu-id="c2078-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2078-114">Application</span></span> | <span data-ttu-id="c2078-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2078-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2078-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2078-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c2078-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2078-117">Request headers</span></span>
| <span data-ttu-id="c2078-118">Name</span><span class="sxs-lookup"><span data-stu-id="c2078-118">Name</span></span>       | <span data-ttu-id="c2078-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c2078-119">Type</span></span> | <span data-ttu-id="c2078-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2078-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2078-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2078-121">Authorization</span></span>  | <span data-ttu-id="c2078-122">string</span><span class="sxs-lookup"><span data-stu-id="c2078-122">string</span></span>  | <span data-ttu-id="c2078-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c2078-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2078-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2078-125">Request body</span></span>
<span data-ttu-id="c2078-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c2078-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2078-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2078-127">Response</span></span>

<span data-ttu-id="c2078-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2078-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2078-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2078-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2078-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2078-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="c2078-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2078-132">Response</span></span>

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