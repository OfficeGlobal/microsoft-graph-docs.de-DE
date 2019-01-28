---
title: Team aus Gruppe erstellen
description: Erstellen eines neuen Teams aus einer Gruppe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a28036cfb253405fab55eca80fa2b0a17232a96c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524793"
---
# <a name="create-team-from-group"></a><span data-ttu-id="86d8f-103">Team aus Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="86d8f-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d8f-104">Erstellen eines neuen [Teams](../resources/team.md) aus einer [Gruppe](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="86d8f-104">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="86d8f-105">Damit ein Team daraus erstellt werden kann, muss die Gruppe mindestens einen Besitzer haben.</span><span class="sxs-lookup"><span data-stu-id="86d8f-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="86d8f-106">Wenn die Gruppe vor weniger als 15 Minuten erstellt wurde, führt der Aufruf zum Erstellen eines Teams möglicherweise zu einem Fehler 404 aufgrund von Verzögerungen bei der Replikation.</span><span class="sxs-lookup"><span data-stu-id="86d8f-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="86d8f-107">Das empfohlene Muster besteht darin, den Aufruf zum Erstellen des Teams drei Mal mit einer Verzögerung von 10 Sekunden zwischen Aufrufen zu wiederholen.</span><span class="sxs-lookup"><span data-stu-id="86d8f-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="86d8f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86d8f-108">Permissions</span></span>

<span data-ttu-id="86d8f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86d8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d8f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86d8f-111">Permission type</span></span>      | <span data-ttu-id="86d8f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86d8f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86d8f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86d8f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="86d8f-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d8f-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86d8f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86d8f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86d8f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86d8f-116">Not supported.</span></span>    |
|<span data-ttu-id="86d8f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86d8f-117">Application</span></span> | <span data-ttu-id="86d8f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d8f-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="86d8f-119">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="86d8f-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="86d8f-120">Globale Administratoren und Microsoft Teams-Dienstadministratoren können auf Gruppen zugreifen, in denen sie kein Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="86d8f-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="86d8f-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d8f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="86d8f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86d8f-122">Request headers</span></span>

| <span data-ttu-id="86d8f-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86d8f-123">Header</span></span>       | <span data-ttu-id="86d8f-124">Wert</span><span class="sxs-lookup"><span data-stu-id="86d8f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86d8f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d8f-125">Authorization</span></span>  | <span data-ttu-id="86d8f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86d8f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="86d8f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86d8f-128">Content-Type</span></span>  | <span data-ttu-id="86d8f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="86d8f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86d8f-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86d8f-130">Request body</span></span>

<span data-ttu-id="86d8f-131">Geben Sie im Anforderungstext eine JSON-Darstellung eines [team](../resources/team.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="86d8f-131">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="86d8f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="86d8f-132">Response</span></span>

<span data-ttu-id="86d8f-133">Bei erfolgreicher Ausführung sollte die Methode den Antwortcode `201 Created` und ein [team](../resources/team.md)-Objekt im Antworttext zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="86d8f-133">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86d8f-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86d8f-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="86d8f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d8f-135">Request</span></span>

<span data-ttu-id="86d8f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86d8f-136">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="86d8f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="86d8f-137">Response</span></span>

<span data-ttu-id="86d8f-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86d8f-138">The following is an example of the response.</span></span> 

><span data-ttu-id="86d8f-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="86d8f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-teams.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="86d8f-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="86d8f-141">See also</span></span>

- [<span data-ttu-id="86d8f-142">Erstellen einer Gruppe mit einem Team</span><span class="sxs-lookup"><span data-stu-id="86d8f-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
