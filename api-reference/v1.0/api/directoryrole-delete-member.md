---
title: Verzeichnisrollenmitglied entfernen
description: Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: a788d9b7ed6b71163bb1b189681cdf7c5fee7575
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850981"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="c14bf-103">Verzeichnisrollenmitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="c14bf-103">Remove directory role member</span></span>

<span data-ttu-id="c14bf-104">Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="c14bf-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="c14bf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c14bf-105">Permissions</span></span>

<span data-ttu-id="c14bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c14bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c14bf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c14bf-108">Permission type</span></span>      | <span data-ttu-id="c14bf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c14bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c14bf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c14bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c14bf-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c14bf-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c14bf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c14bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c14bf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c14bf-113">Not supported.</span></span>    |
|<span data-ttu-id="c14bf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c14bf-114">Application</span></span> | <span data-ttu-id="c14bf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c14bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c14bf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c14bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c14bf-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c14bf-117">Request headers</span></span>

| <span data-ttu-id="c14bf-118">Name</span><span class="sxs-lookup"><span data-stu-id="c14bf-118">Name</span></span>       | <span data-ttu-id="c14bf-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c14bf-119">Type</span></span> | <span data-ttu-id="c14bf-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c14bf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c14bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c14bf-121">Authorization</span></span>  | <span data-ttu-id="c14bf-122">string</span><span class="sxs-lookup"><span data-stu-id="c14bf-122">string</span></span>  | <span data-ttu-id="c14bf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c14bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c14bf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c14bf-125">Request body</span></span>

<span data-ttu-id="c14bf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c14bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c14bf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c14bf-127">Response</span></span>

<span data-ttu-id="c14bf-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c14bf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c14bf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c14bf-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c14bf-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c14bf-131">Request</span></span>

<span data-ttu-id="c14bf-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c14bf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="c14bf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c14bf-133">Response</span></span>

<span data-ttu-id="c14bf-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c14bf-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
