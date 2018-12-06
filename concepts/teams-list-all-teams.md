---
title: Auflisten aller Teams einer Organisation in Microsoft Teams
description: 'Auflisten aller Teams '
ms.openlocfilehash: 2a9dbaa1fc9a02897870865295fd8d0dac9266a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092267"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a><span data-ttu-id="a589d-103">Auflisten aller Teams einer Organisation in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a589d-103">List all teams in Microsoft Teams for an organization</span></span>

<span data-ttu-id="a589d-104">Um alle [Teams](/graph/api/resources/team?view=graph-rest-beta) in einer Organisation (einem Mandanten) aufzulisten, suchen Sie alle Gruppen, die über Teams verfügen und rufen dann Informationen für jedes Team ab.</span><span class="sxs-lookup"><span data-stu-id="a589d-104">To list all [teams](/graph/api/resources/team?view=graph-rest-beta) in an organization (tenant), you find all groups that have teams, and then get information for each team.</span></span>

## <a name="get-a-list-of-groups"></a><span data-ttu-id="a589d-105">Abrufen einer Liste von Gruppen</span><span class="sxs-lookup"><span data-stu-id="a589d-105">Get a collection of section groups.</span></span>

<span data-ttu-id="a589d-106">Um eine Liste aller [Gruppen](/graph/api/resources/group?view=graph-rest-beta) in der Organisation abzurufen, die über Teams verfügen, rufen Sie eine [Liste aller Gruppen](/graph/api/group-list?view=graph-rest-beta) ab, und suchen Sie dann im Code diejenigen Gruppen, deren Eigenschaft **resourceProvisioningOptions** "Team" enthält.</span><span class="sxs-lookup"><span data-stu-id="a589d-106">To get a list of all [groups](/graph/api/resources/group?view=graph-rest-beta) in the organization that have teams, get a [list of all groups](/graph/api/group-list?view=graph-rest-beta) and then in code find the ones that have a **resourceProvisioningOptions** property that contains "Team".</span></span>
<span data-ttu-id="a589d-107">Da es sich bei Gruppen um große Objekte handelt, verwenden Sie "$select", um nur die Eigenschaften der in Frage kommenden Gruppe abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a589d-107">Since groups are large objects, use $select to only get the properties of the group you care about.</span></span>

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> <span data-ttu-id="a589d-108">**Hinweis**: Bei einigen nicht verwendeten alten Teams ist die Eigenschaft "resourceProvisioningOptions" nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a589d-108">**Note**: Certain unused old teams will not have resourceProvisioningOptions set.</span></span> <span data-ttu-id="a589d-109">Einzelheiten hierzu finden Sie unter [bekannte Probleme](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="a589d-109">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="a589d-110">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a589d-110">The following is an example of the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "00e897b1-70ba-4cb9-9126-fd5f95c4bb78",
            "resourceProvisioningOptions": []
        },
        {
            "id": "00f6e045-f884-4359-a617-d459ee626862",
            "resourceProvisioningOptions": [
                "Team"
            ]
        }
    ]
}
```

## <a name="get-a-list-of-groups-using-beta-apis"></a><span data-ttu-id="a589d-111">Abrufen einer Liste der Gruppen mit Beta-APIs</span><span class="sxs-lookup"><span data-stu-id="a589d-111">Get a list of groups using beta APIs</span></span>

<span data-ttu-id="a589d-112">Mithilfe der Beta-APIs können Sie "$filter" verwenden, um nur die Gruppen zurückzugeben, die über Teams verfügen.</span><span class="sxs-lookup"><span data-stu-id="a589d-112">Using the beta APIs, you can use $filter to return only the groups that have teams.</span></span>

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> <span data-ttu-id="a589d-113">**Hinweis**: "$filter" ist für "/groups" nur über den Beta-Endpunkt verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a589d-113">**Note**: $filter on /groups is only available through the beta endpoint.</span></span> <span data-ttu-id="a589d-114">"resourceProvisioningOptions" ist in v1.0 und in der Beta verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a589d-114">resourceProvisioningOptions is available in v1.0 and beta.</span></span>

> <span data-ttu-id="a589d-115">**Hinweis**: Bestimmte nicht verwendete alte Teams werden nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="a589d-115">**Note**: Certain unused old teams will not be listed.</span></span> <span data-ttu-id="a589d-116">Einzelheiten hierzu finden Sie unter [bekannte Probleme](known-issues.md#missing-teams-in-list-all-teams).</span><span class="sxs-lookup"><span data-stu-id="a589d-116">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="a589d-117">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a589d-117">The following is an example of the response.</span></span> 

><span data-ttu-id="a589d-118">**Hinweis:** Das gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="a589d-118">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a589d-119">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a589d-119">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
    "value": [
        {
            "id": "02bd9fd6-8f93-4758-87c3-1fb73740a315",
            "description": "Welcome to the HR Taskforce team.",
            "displayName": "HR Taskforce",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "HRTaskforce",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private",
        },
        {
            "id": "8090c93e-ba7c-433e-9f39-08c7ba07c0b3",
            "description": "Welcome to the team that we've assembled to launch our product.",
            "displayName": "X1050 Launch Team",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "X1050LaunchTeam",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private",
        }
    ]
}
```

## <a name="get-team-information-for-a-group"></a><span data-ttu-id="a589d-120">Abrufen von Teaminformationen für eine Gruppe</span><span class="sxs-lookup"><span data-stu-id="a589d-120">Get team information for a group</span></span>

<span data-ttu-id="a589d-121">Um Teaminformationen für das Team in einer bestimmten Gruppe abzurufen, rufen Sie die [get team](/graph/api/team-get?view=graph-rest-beta)-API auf, und schließen Sie die Gruppen-ID ein.</span><span class="sxs-lookup"><span data-stu-id="a589d-121">To get team information for the team in a particular group, call the [get team](/graph/api/team-get?view=graph-rest-beta) API and include the group ID.</span></span>

```http
GET /teams/{group-id}
```

<span data-ttu-id="a589d-122">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="a589d-122">The following example shows the response.</span></span>

><span data-ttu-id="a589d-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a589d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a589d-125">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a589d-125">See also</span></span>

- [<span data-ttu-id="a589d-126">joinedTeams auflisten</span><span class="sxs-lookup"><span data-stu-id="a589d-126">List joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [<span data-ttu-id="a589d-127">Gruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="a589d-127">List groups</span></span>](/graph/api/group-list?view=graph-rest-beta)
