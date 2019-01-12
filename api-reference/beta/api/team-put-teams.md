---
title: Erstellen von Teams aus Gruppe
description: Erstellen Sie ein neues Team aus einer Gruppe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 277a889201f6a161b2ed4191721616a11ead2f41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938692"
---
# <a name="create-team-from-group"></a><span data-ttu-id="3a71d-103">Erstellen von Teams aus Gruppe</span><span class="sxs-lookup"><span data-stu-id="3a71d-103">Create team from group</span></span>

> <span data-ttu-id="3a71d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a71d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a71d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a71d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a71d-106">Erstellen Sie ein neues [Team](../resources/team.md) aus einer [Gruppe](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3a71d-106">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="3a71d-107">Um ein Team zu erstellen, muss die Gruppe einen mindestens einen Besitzer haben.</span><span class="sxs-lookup"><span data-stu-id="3a71d-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="3a71d-108">Wenn die Gruppe vor weniger als 15 Minuten erstellt wurde, kann der erstellen teamanruf an einen Code 404-Fehler aufgrund von Replikation Verzögerungen auftreten.</span><span class="sxs-lookup"><span data-stu-id="3a71d-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="3a71d-109">Das empfohlene Muster liegt, um den Aufruf der Create-Team drei Mal mit einer Verzögerung von 10 Sekunden zwischen aufrufen.</span><span class="sxs-lookup"><span data-stu-id="3a71d-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a71d-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a71d-110">Permissions</span></span>

<span data-ttu-id="3a71d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a71d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a71d-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a71d-113">Permission type</span></span>      | <span data-ttu-id="3a71d-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a71d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a71d-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a71d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3a71d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a71d-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a71d-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a71d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a71d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a71d-118">Not supported.</span></span>    |
|<span data-ttu-id="3a71d-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a71d-119">Application</span></span> | <span data-ttu-id="3a71d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a71d-120">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="3a71d-121">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="3a71d-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3a71d-122">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Gruppen zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="3a71d-122">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a71d-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a71d-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="3a71d-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a71d-124">Request headers</span></span>

| <span data-ttu-id="3a71d-125">Header</span><span class="sxs-lookup"><span data-stu-id="3a71d-125">Header</span></span>       | <span data-ttu-id="3a71d-126">Wert</span><span class="sxs-lookup"><span data-stu-id="3a71d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a71d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a71d-127">Authorization</span></span>  | <span data-ttu-id="3a71d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a71d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a71d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a71d-130">Content-Type</span></span>  | <span data-ttu-id="3a71d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3a71d-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a71d-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a71d-132">Request body</span></span>

<span data-ttu-id="3a71d-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3a71d-133">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3a71d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a71d-134">Response</span></span>

<span data-ttu-id="3a71d-135">Wenn diese Methode erfolgreich ist, zurückgeben soll eine `201 Created` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a71d-135">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a71d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a71d-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3a71d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a71d-137">Request</span></span>

<span data-ttu-id="3a71d-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a71d-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/beta/groups/{id}/team
Content-type: application/json

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

#### <a name="response"></a><span data-ttu-id="3a71d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a71d-139">Response</span></span>

<span data-ttu-id="3a71d-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a71d-140">The following is an example of the response.</span></span> 

><span data-ttu-id="3a71d-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3a71d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="3a71d-143">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3a71d-143">See also</span></span>

- [<span data-ttu-id="3a71d-144">Erstellen einer Gruppe mit einem team</span><span class="sxs-lookup"><span data-stu-id="3a71d-144">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
