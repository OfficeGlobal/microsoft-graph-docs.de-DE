---
title: Team erstellen
description: Erstellt ein neues Team.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3e901225f5a8f94abb61a6b4052b0db2d47865c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519612"
---
# <a name="create-team"></a><span data-ttu-id="bd04d-103">Team erstellen</span><span class="sxs-lookup"><span data-stu-id="bd04d-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd04d-104">Erstellt ein neues [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bd04d-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd04d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd04d-105">Permissions</span></span>

<span data-ttu-id="bd04d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd04d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd04d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd04d-108">Permission type</span></span>                        | <span data-ttu-id="bd04d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd04d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bd04d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd04d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd04d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd04d-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="bd04d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd04d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd04d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd04d-113">Not supported.</span></span>                              |
| <span data-ttu-id="bd04d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd04d-114">Application</span></span>                            | <span data-ttu-id="bd04d-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd04d-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bd04d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd04d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="bd04d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd04d-117">Request headers</span></span>

| <span data-ttu-id="bd04d-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd04d-118">Header</span></span>        | <span data-ttu-id="bd04d-119">Wert</span><span class="sxs-lookup"><span data-stu-id="bd04d-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="bd04d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd04d-120">Authorization</span></span> | <span data-ttu-id="bd04d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd04d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd04d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd04d-123">Content-Type</span></span>  | <span data-ttu-id="bd04d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd04d-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="bd04d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd04d-125">Request body</span></span>

<span data-ttu-id="bd04d-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [team](../resources/team.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bd04d-126">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bd04d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd04d-127">Response</span></span>

<span data-ttu-id="bd04d-128">Falls erfolgreich, gibt diese API eine `202 Accepted`-Antwort mit einem Link zu [teamsAsyncOperation](../resources/teamsasyncoperation.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="bd04d-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="bd04d-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bd04d-129">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="bd04d-130">Beispiel zu delegierten Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd04d-130">Example - delegated permissions</span></span>

<span data-ttu-id="bd04d-131">Nachfolgend finden Sie ein Beispiel für eine Mindestanforderung.</span><span class="sxs-lookup"><span data-stu-id="bd04d-131">Here is an example of a minimal request.</span></span> <span data-ttu-id="bd04d-132">Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="bd04d-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="bd04d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd04d-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="bd04d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd04d-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="bd04d-135">Beispiel: Erstellen eines Teams mit einer App, mehreren Kanälen mit angehefteten Registerkarten unter Verwendung delegierter Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd04d-135">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="bd04d-136">Im Folgenden sehen Sie eine Anforderung mit vollständiger Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="bd04d-136">Here is request with a full payload.</span></span> <span data-ttu-id="bd04d-137">Der Client kann Werte in der Basisvorlage außer Kraft setzen und zu Elementen mit Arraywerten hinzufügen, soweit es die Validierungsregeln für `specialization` zulassen.</span><span class="sxs-lookup"><span data-stu-id="bd04d-137">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="bd04d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd04d-138">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="bd04d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd04d-139">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="bd04d-140">Beispiel für Anwendungsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd04d-140">Example - application permissions</span></span>

<span data-ttu-id="bd04d-141">Im Folgenden sehen Sie ein Beispiel für eine Mindestanforderung unter Verwendung der Anwendungsberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="bd04d-141">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="bd04d-142">Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="bd04d-142">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="bd04d-143">Wenn Sie eine Anforderung mit Anwendungsberechtigungen erstellen, muss ein [Benutzer](../resources/user.md) in der `owners`-Sammlung angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="bd04d-143">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="bd04d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd04d-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="bd04d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd04d-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="bd04d-146">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="bd04d-146">See also</span></span>

- [<span data-ttu-id="bd04d-147">Erstellen einer Gruppe mit einem Team</span><span class="sxs-lookup"><span data-stu-id="bd04d-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/team-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
