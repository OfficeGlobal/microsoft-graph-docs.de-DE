---
title: Verzeichnisrollenmitglied entfernen
description: Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.
author: lleonard-msft
ms.openlocfilehash: a0c2976fdab3e548e9bf27cc19b7049926562ea7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350533"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="74573-103">Verzeichnisrollenmitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="74573-103">Remove directory role member</span></span>

<span data-ttu-id="74573-104">Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="74573-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="74573-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74573-105">Permissions</span></span>

<span data-ttu-id="74573-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="74573-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74573-108">Permission type</span></span>      | <span data-ttu-id="74573-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74573-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74573-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74573-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74573-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74573-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74573-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74573-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74573-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74573-113">Not supported.</span></span>    |
|<span data-ttu-id="74573-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74573-114">Application</span></span> | <span data-ttu-id="74573-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74573-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74573-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74573-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="74573-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74573-117">Request headers</span></span>

| <span data-ttu-id="74573-118">Name</span><span class="sxs-lookup"><span data-stu-id="74573-118">Name</span></span>       | <span data-ttu-id="74573-119">Typ</span><span class="sxs-lookup"><span data-stu-id="74573-119">Type</span></span> | <span data-ttu-id="74573-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74573-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74573-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="74573-121">Authorization</span></span>  | <span data-ttu-id="74573-122">string</span><span class="sxs-lookup"><span data-stu-id="74573-122">string</span></span>  | <span data-ttu-id="74573-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74573-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74573-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74573-125">Request body</span></span>

<span data-ttu-id="74573-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="74573-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74573-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="74573-127">Response</span></span>

<span data-ttu-id="74573-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74573-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74573-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74573-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="74573-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74573-131">Request</span></span>

<span data-ttu-id="74573-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74573-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="74573-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="74573-133">Response</span></span>

<span data-ttu-id="74573-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74573-134">Here is an example of the response.</span></span> 
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