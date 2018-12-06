---
title: Erstellen einer Gruppe mit einem Microsoft Teams-Team
description: 'Das Erstellen einer Gruppe, die ein Team umfasst, beinhaltet zwei Schritte: '
ms.openlocfilehash: 530b3625a1aa1d020bff841196e3b83a2eb99a4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092211"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="eb5e0-103">Erstellen einer Gruppe mit einem Microsoft Teams-Team</span><span class="sxs-lookup"><span data-stu-id="eb5e0-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="eb5e0-104">Das Erstellen einer [Gruppe](/graph/api/resources/group?view=graph-rest-beta), die ein [Team](/graph/api/resources/team?view=graph-rest-beta) umfasst, beinhaltet zwei Schritte:</span><span class="sxs-lookup"><span data-stu-id="eb5e0-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="eb5e0-105">Das [Erstellen einer Gruppe](/graph/api/group-post-groups?view=graph-rest-beta) mit den richtigen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="eb5e0-106">Das [Hinzufügen eines Teams](/graph/api/team-put-teams?view=graph-rest-beta) zur Gruppe.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="eb5e0-107">Erstellen einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="eb5e0-107">Create a group:</span></span>

<span data-ttu-id="eb5e0-108">Um ein Team einzuschließen, müssen Sie die folgenden Eigenschaftswerte festlegen, wie im folgenden Beispiel gezeigt:</span><span class="sxs-lookup"><span data-stu-id="eb5e0-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="eb5e0-109">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="eb5e0-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="eb5e0-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="eb5e0-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="eb5e0-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="eb5e0-111">**securityEnabled** = false</span></span>

```http
POST /groups
{
    "displayName":"Flight 157",
    "mailNickname":"flight157",
    "description":"Everything about flight 157",
    "visibility":"Private",
    "groupTypes":["Unified"],
    "mailEnabled":true,
    "securityEnabled":false,
    "members@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
        "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
    ],
    "owners@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
    ]
}
```

<span data-ttu-id="eb5e0-112">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-112">The following example shows the response.</span></span> 

><span data-ttu-id="eb5e0-113">**Hinweis:** Das gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-113">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb5e0-114">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="eb5e0-115">Hinzufügen eines Teams zur Gruppe</span><span class="sxs-lookup"><span data-stu-id="eb5e0-115">Add a team to the group</span></span>

<span data-ttu-id="eb5e0-116">Fügen Sie der Gruppe, wie dargestellt, ein Team hinzu.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="eb5e0-117">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-117">The following example shows the response.</span></span> 

><span data-ttu-id="eb5e0-118">**Hinweis:** Das gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-118">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb5e0-119">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-119">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
    "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
    "webUrl" : "https://example.com",
    "isArchived" : null,
    "memberSettings" : { },
    "guestSettings" : { },
    "messagingSettings" : { },
    "funSettings" : {}
}
```

<span data-ttu-id="eb5e0-120">Das erstellte Team hat die gleiche ID wie die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="eb5e0-120">The created team has the same ID as the group.</span></span>
