---
title: Update-team
description: Aktualisieren Sie die Eigenschaften des angegebenen Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1185ad9d835f660c98d12fac8472bd6325463858
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991874"
---
# <a name="update-team"></a><span data-ttu-id="4a9ea-103">Update-team</span><span class="sxs-lookup"><span data-stu-id="4a9ea-103">Update team</span></span>



<span data-ttu-id="4a9ea-104">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4a9ea-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a9ea-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a9ea-105">Permissions</span></span>
<span data-ttu-id="4a9ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a9ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a9ea-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a9ea-108">Permission type</span></span>      | <span data-ttu-id="4a9ea-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a9ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a9ea-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a9ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a9ea-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a9ea-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a9ea-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a9ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a9ea-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a9ea-113">Not supported.</span></span>    |
|<span data-ttu-id="4a9ea-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a9ea-114">Application</span></span> | <span data-ttu-id="4a9ea-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a9ea-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="4a9ea-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4a9ea-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a9ea-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a9ea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a9ea-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a9ea-119">Request headers</span></span>
| <span data-ttu-id="4a9ea-120">Header</span><span class="sxs-lookup"><span data-stu-id="4a9ea-120">Header</span></span>       | <span data-ttu-id="4a9ea-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4a9ea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a9ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a9ea-122">Authorization</span></span>  | <span data-ttu-id="4a9ea-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4a9ea-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a9ea-125">Content-Type</span></span>  | <span data-ttu-id="4a9ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a9ea-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a9ea-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a9ea-127">Request body</span></span>
<span data-ttu-id="4a9ea-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4a9ea-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a9ea-129">Response</span></span>

<span data-ttu-id="4a9ea-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4a9ea-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a9ea-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4a9ea-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a9ea-132">Request</span></span>
<span data-ttu-id="4a9ea-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a9ea-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="4a9ea-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a9ea-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
