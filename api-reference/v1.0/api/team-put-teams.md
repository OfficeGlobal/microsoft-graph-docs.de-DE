---
title: Erstellen von Teams
description: Erstellen Sie ein neues Team unter einer Gruppe.
author: nkramer
ms.openlocfilehash: 5bda73b667d23065bf8500346e7ce188dac318c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361705"
---
# <a name="create-team"></a><span data-ttu-id="14092-103">Erstellen von Teams</span><span class="sxs-lookup"><span data-stu-id="14092-103">Create team</span></span>



<span data-ttu-id="14092-104">Erstellen Sie ein neues [Team](../resources/team.md) unter einer [Gruppe](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="14092-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="14092-105">Um ein Team zu erstellen, muss die Gruppe einen mindestens einen Besitzer haben.</span><span class="sxs-lookup"><span data-stu-id="14092-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="14092-106">Wenn die Gruppe vor weniger als 15 Minuten erstellt wurde, kann der erstellen teamanruf an einen Code 404-Fehler aufgrund von Replikation Verzögerungen auftreten.</span><span class="sxs-lookup"><span data-stu-id="14092-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="14092-107">Das empfohlene Muster liegt, um den Aufruf der Create-Team drei Mal mit einer Verzögerung von 10 Sekunden zwischen aufrufen.</span><span class="sxs-lookup"><span data-stu-id="14092-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="14092-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="14092-108">Permissions</span></span>

<span data-ttu-id="14092-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14092-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14092-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14092-111">Permission type</span></span>      | <span data-ttu-id="14092-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14092-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14092-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14092-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14092-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14092-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14092-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14092-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14092-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14092-116">Not supported.</span></span>    |
|<span data-ttu-id="14092-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14092-117">Application</span></span> | <span data-ttu-id="14092-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14092-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="14092-119">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="14092-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14092-120">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Gruppen zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="14092-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="14092-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14092-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="14092-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14092-122">Request headers</span></span>

| <span data-ttu-id="14092-123">Header</span><span class="sxs-lookup"><span data-stu-id="14092-123">Header</span></span>       | <span data-ttu-id="14092-124">Wert</span><span class="sxs-lookup"><span data-stu-id="14092-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14092-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14092-125">Authorization</span></span>  | <span data-ttu-id="14092-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14092-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14092-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14092-128">Content-Type</span></span>  | <span data-ttu-id="14092-129">application/json</span><span class="sxs-lookup"><span data-stu-id="14092-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14092-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14092-130">Request body</span></span>

<span data-ttu-id="14092-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="14092-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="14092-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="14092-132">Response</span></span>

<span data-ttu-id="14092-133">Wenn diese Methode erfolgreich ist, zurückgeben soll eine `201 Created` Antwortcode und ein [Team](../resources/team.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14092-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14092-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14092-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="14092-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14092-135">Request</span></span>

<span data-ttu-id="14092-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14092-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
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

#### <a name="response"></a><span data-ttu-id="14092-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="14092-137">Response</span></span>

<span data-ttu-id="14092-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14092-138">The following is an example of the response.</span></span> 

><span data-ttu-id="14092-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="14092-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="14092-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="14092-141">See also</span></span>

- [<span data-ttu-id="14092-142">Erstellen einer Gruppe mit einem team</span><span class="sxs-lookup"><span data-stu-id="14092-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
