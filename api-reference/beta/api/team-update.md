---
title: Update-team
description: Aktualisieren Sie die Eigenschaften des angegebenen Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f70c3212fb3297158f060d37f2f5906b62139a7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507614"
---
# <a name="update-team"></a><span data-ttu-id="2f2f2-103">Update-team</span><span class="sxs-lookup"><span data-stu-id="2f2f2-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f2f2-104">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2f2f2-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f2f2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f2f2-105">Permissions</span></span>
<span data-ttu-id="2f2f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2f2f2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f2f2-108">Permission type</span></span>      | <span data-ttu-id="2f2f2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f2f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f2f2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f2f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f2f2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2f2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f2f2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f2f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f2f2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f2f2-113">Not supported.</span></span>    |
|<span data-ttu-id="2f2f2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f2f2-114">Application</span></span> | <span data-ttu-id="2f2f2-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2f2-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="2f2f2-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2f2f2-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f2f2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f2f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2f2f2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f2f2-119">Request headers</span></span>
| <span data-ttu-id="2f2f2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f2f2-120">Header</span></span>       | <span data-ttu-id="2f2f2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2f2f2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f2f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f2f2-122">Authorization</span></span>  | <span data-ttu-id="2f2f2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f2f2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f2f2-125">Content-Type</span></span>  | <span data-ttu-id="2f2f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2f2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f2f2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f2f2-127">Request body</span></span>
<span data-ttu-id="2f2f2-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f2f2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f2f2-129">Response</span></span>

<span data-ttu-id="2f2f2-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f2f2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f2f2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2f2f2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f2f2-132">Request</span></span>
<span data-ttu-id="2f2f2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f2f2-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="2f2f2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f2f2-134">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
