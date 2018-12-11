---
title: Get-team
description: Abrufen der Eigenschaften und Beziehungen zwischen dem angegebenen Team.
ms.openlocfilehash: e1f3b08134377492fc00f9bc0b43c190d1d8a81d
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222646"
---
# <a name="get-team"></a><span data-ttu-id="fd627-103">Get-team</span><span class="sxs-lookup"><span data-stu-id="fd627-103">Get team</span></span>



<span data-ttu-id="fd627-104">Abrufen der Eigenschaften und Beziehungen des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fd627-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd627-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd627-105">Permissions</span></span>
<span data-ttu-id="fd627-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd627-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd627-108">Permission type</span></span>      | <span data-ttu-id="fd627-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd627-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd627-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd627-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd627-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd627-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd627-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd627-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd627-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd627-113">Not supported.</span></span>    |
|<span data-ttu-id="fd627-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd627-114">Application</span></span> | <span data-ttu-id="fd627-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd627-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="fd627-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="fd627-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fd627-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="fd627-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd627-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd627-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd627-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd627-119">Optional query parameters</span></span>
<span data-ttu-id="fd627-120">Diese Methode unterstützt die $select und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="fd627-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd627-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd627-121">Request headers</span></span>
| <span data-ttu-id="fd627-122">Header</span><span class="sxs-lookup"><span data-stu-id="fd627-122">Header</span></span>       | <span data-ttu-id="fd627-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fd627-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd627-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd627-124">Authorization</span></span>  | <span data-ttu-id="fd627-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd627-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd627-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd627-127">Request body</span></span>
<span data-ttu-id="fd627-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd627-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd627-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd627-129">Response</span></span>

<span data-ttu-id="fd627-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd627-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd627-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd627-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fd627-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd627-132">Request</span></span>
<span data-ttu-id="fd627-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd627-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="fd627-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd627-134">Response</span></span>
<span data-ttu-id="fd627-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd627-135">The following is an example of the response.</span></span> 

><span data-ttu-id="fd627-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fd627-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
