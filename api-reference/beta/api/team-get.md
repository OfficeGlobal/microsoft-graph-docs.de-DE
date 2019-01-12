---
title: Get-team
description: Abrufen der Eigenschaften und Beziehungen zwischen dem angegebenen Team.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 4ec9c53dbb474afabc3c2a67e480bf9972dfefc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947708"
---
# <a name="get-team"></a><span data-ttu-id="a7934-103">Get-team</span><span class="sxs-lookup"><span data-stu-id="a7934-103">Get team</span></span>

> <span data-ttu-id="a7934-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7934-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7934-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7934-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7934-106">Abrufen der Eigenschaften und Beziehungen des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a7934-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7934-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a7934-107">Permissions</span></span>
<span data-ttu-id="a7934-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7934-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7934-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7934-110">Permission type</span></span>      | <span data-ttu-id="a7934-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7934-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7934-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7934-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a7934-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7934-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7934-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7934-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7934-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7934-115">Not supported.</span></span>    |
|<span data-ttu-id="a7934-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7934-116">Application</span></span> | <span data-ttu-id="a7934-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7934-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a7934-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="a7934-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a7934-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="a7934-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7934-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7934-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7934-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a7934-121">Optional query parameters</span></span>
<span data-ttu-id="a7934-122">Diese Methode unterstützt die $select und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="a7934-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7934-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7934-123">Request headers</span></span>
| <span data-ttu-id="a7934-124">Header</span><span class="sxs-lookup"><span data-stu-id="a7934-124">Header</span></span>       | <span data-ttu-id="a7934-125">Wert</span><span class="sxs-lookup"><span data-stu-id="a7934-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7934-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7934-126">Authorization</span></span>  | <span data-ttu-id="a7934-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7934-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7934-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7934-129">Request body</span></span>
<span data-ttu-id="a7934-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a7934-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7934-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7934-131">Response</span></span>

<span data-ttu-id="a7934-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a7934-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7934-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7934-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a7934-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7934-134">Request</span></span>
<span data-ttu-id="a7934-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7934-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="a7934-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7934-136">Response</span></span>
<span data-ttu-id="a7934-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a7934-137">The following is an example of the response.</span></span> 

><span data-ttu-id="a7934-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a7934-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
