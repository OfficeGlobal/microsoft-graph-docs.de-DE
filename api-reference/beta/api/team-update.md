---
title: Update-team
description: Aktualisieren Sie die Eigenschaften des angegebenen Teams.
ms.openlocfilehash: e5148b21fa832c45e1f89c1296fd0df64aaf71e0
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222478"
---
# <a name="update-team"></a><span data-ttu-id="9905b-103">Update-team</span><span class="sxs-lookup"><span data-stu-id="9905b-103">Update team</span></span>

> <span data-ttu-id="9905b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9905b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9905b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9905b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9905b-106">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9905b-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9905b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9905b-107">Permissions</span></span>
<span data-ttu-id="9905b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9905b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9905b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9905b-110">Permission type</span></span>      | <span data-ttu-id="9905b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9905b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9905b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9905b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9905b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9905b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9905b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9905b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9905b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9905b-115">Not supported.</span></span>    |
|<span data-ttu-id="9905b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9905b-116">Application</span></span> | <span data-ttu-id="9905b-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9905b-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="9905b-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="9905b-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9905b-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="9905b-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9905b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9905b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9905b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9905b-121">Request headers</span></span>
| <span data-ttu-id="9905b-122">Header</span><span class="sxs-lookup"><span data-stu-id="9905b-122">Header</span></span>       | <span data-ttu-id="9905b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9905b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9905b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9905b-124">Authorization</span></span>  | <span data-ttu-id="9905b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9905b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9905b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9905b-127">Content-Type</span></span>  | <span data-ttu-id="9905b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9905b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9905b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9905b-129">Request body</span></span>
<span data-ttu-id="9905b-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9905b-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9905b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9905b-131">Response</span></span>

<span data-ttu-id="9905b-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9905b-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9905b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9905b-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9905b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9905b-134">Request</span></span>
<span data-ttu-id="9905b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9905b-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="9905b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9905b-136">Response</span></span>
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
