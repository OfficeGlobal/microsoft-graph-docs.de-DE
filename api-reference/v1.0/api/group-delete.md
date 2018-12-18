---
title: Gruppe löschen
description: Mit dieser API können Sie Gruppen löschen.
author: dkershaw10
ms.openlocfilehash: 6377c3d7865ebcc1ef13a649afbde083163e7048
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326278"
---
# <a name="delete-group"></a><span data-ttu-id="44704-103">Gruppe löschen</span><span class="sxs-lookup"><span data-stu-id="44704-103">Delete group</span></span>
<span data-ttu-id="44704-104">Mit dieser API können Sie Gruppen löschen.</span><span class="sxs-lookup"><span data-stu-id="44704-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="44704-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44704-105">Permissions</span></span>
<span data-ttu-id="44704-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44704-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44704-108">Permission type</span></span>      | <span data-ttu-id="44704-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44704-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44704-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44704-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44704-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44704-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44704-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44704-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44704-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44704-113">Not supported.</span></span>    |
|<span data-ttu-id="44704-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44704-114">Application</span></span> | <span data-ttu-id="44704-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44704-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44704-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44704-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44704-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44704-117">Request headers</span></span>
| <span data-ttu-id="44704-118">Name</span><span class="sxs-lookup"><span data-stu-id="44704-118">Name</span></span>       | <span data-ttu-id="44704-119">Typ</span><span class="sxs-lookup"><span data-stu-id="44704-119">Type</span></span> | <span data-ttu-id="44704-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44704-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44704-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="44704-121">Authorization</span></span>  | <span data-ttu-id="44704-122">string</span><span class="sxs-lookup"><span data-stu-id="44704-122">string</span></span>  | <span data-ttu-id="44704-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44704-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44704-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44704-125">Request body</span></span>
<span data-ttu-id="44704-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44704-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44704-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="44704-127">Response</span></span>
<span data-ttu-id="44704-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44704-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44704-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44704-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="44704-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44704-131">Request</span></span>
<span data-ttu-id="44704-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44704-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="44704-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="44704-133">Response</span></span>
<span data-ttu-id="44704-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44704-134">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->