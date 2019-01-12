---
title: Update-team
description: Aktualisieren Sie die Eigenschaften des angegebenen Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb882a31916d31744d57cdc0ef3d2a161361b628
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925987"
---
# <a name="update-team"></a><span data-ttu-id="aa51a-103">Update-team</span><span class="sxs-lookup"><span data-stu-id="aa51a-103">Update team</span></span>

> <span data-ttu-id="aa51a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa51a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa51a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa51a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa51a-106">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="aa51a-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa51a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa51a-107">Permissions</span></span>
<span data-ttu-id="aa51a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa51a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aa51a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa51a-110">Permission type</span></span>      | <span data-ttu-id="aa51a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa51a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa51a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa51a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa51a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa51a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa51a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa51a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa51a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa51a-115">Not supported.</span></span>    |
|<span data-ttu-id="aa51a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa51a-116">Application</span></span> | <span data-ttu-id="aa51a-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa51a-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="aa51a-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="aa51a-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aa51a-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="aa51a-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa51a-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa51a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="aa51a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa51a-121">Request headers</span></span>
| <span data-ttu-id="aa51a-122">Header</span><span class="sxs-lookup"><span data-stu-id="aa51a-122">Header</span></span>       | <span data-ttu-id="aa51a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="aa51a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa51a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa51a-124">Authorization</span></span>  | <span data-ttu-id="aa51a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa51a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aa51a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa51a-127">Content-Type</span></span>  | <span data-ttu-id="aa51a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aa51a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa51a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa51a-129">Request body</span></span>
<span data-ttu-id="aa51a-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa51a-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aa51a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa51a-131">Response</span></span>

<span data-ttu-id="aa51a-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa51a-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa51a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa51a-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aa51a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa51a-134">Request</span></span>
<span data-ttu-id="aa51a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa51a-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="aa51a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa51a-136">Response</span></span>
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
