---
title: Erstellen eines Teams
description: Erstellen Sie ein neues Team.
author: nkramer
ms.openlocfilehash: c77ca5ab76640c9c310b628f4eee106e7443fee7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362839"
---
# <a name="create-team"></a><span data-ttu-id="7c6b1-103">Erstellen von Teams</span><span class="sxs-lookup"><span data-stu-id="7c6b1-103">Create team</span></span>

> <span data-ttu-id="7c6b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c6b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c6b1-106">Erstellen Sie ein neues [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7c6b1-106">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c6b1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c6b1-107">Permissions</span></span>

<span data-ttu-id="7c6b1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c6b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c6b1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c6b1-110">Permission type</span></span>                        | <span data-ttu-id="7c6b1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c6b1-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7c6b1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c6b1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c6b1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6b1-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="7c6b1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c6b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c6b1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c6b1-115">Not supported.</span></span>                              |
| <span data-ttu-id="7c6b1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c6b1-116">Application</span></span>                            | <span data-ttu-id="7c6b1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6b1-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c6b1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6b1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="7c6b1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c6b1-119">Request headers</span></span>

| <span data-ttu-id="7c6b1-120">Header</span><span class="sxs-lookup"><span data-stu-id="7c6b1-120">Header</span></span>        | <span data-ttu-id="7c6b1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7c6b1-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7c6b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c6b1-122">Authorization</span></span> | <span data-ttu-id="7c6b1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c6b1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c6b1-125">Content-Type</span></span>  | <span data-ttu-id="7c6b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c6b1-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="7c6b1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c6b1-127">Request body</span></span>

<span data-ttu-id="7c6b1-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-128">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7c6b1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6b1-129">Response</span></span>

<span data-ttu-id="7c6b1-130">Wenn erfolgreich, diese API gibt eine `202 Accepted` mit einem Link zu der [TeamsAsyncOperation](../resources/teamsasyncoperation.md)Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-130">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="7c6b1-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="7c6b1-131">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="7c6b1-132">Beispiel - delegierten Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c6b1-132">Example - delegated permissions</span></span>

<span data-ttu-id="7c6b1-133">Hier ist ein Beispiel für eine minimale Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-133">Here is an example of a minimal request.</span></span> <span data-ttu-id="7c6b1-134">Durch andere Eigenschaften auslassen, ist der Client implizit Standardwerte aus der vordefinierten Vorlage dargestellt durch Offlineschalten `template`.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-134">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="7c6b1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6b1-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="7c6b1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6b1-136">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="7c6b1-137">Beispiel: Erstellen Sie ein Team mit einer app installiert, mehrere Kanäle mit angeheftete Registerkarten von delegierten Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c6b1-137">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="7c6b1-138">Es folgt Anforderung mit einer vollständigen Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-138">Here is request with a full payload.</span></span> <span data-ttu-id="7c6b1-139">Der Client-Werte in der Basisvorlage außer Kraft und Elementen durch Überprüfungsregeln für zulässigen soweit Array wiederholendem hinzufügen kann die `specialization`.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-139">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="7c6b1-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6b1-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7c6b1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6b1-141">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="7c6b1-142">Beispiel - Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c6b1-142">Example - application permissions</span></span>

<span data-ttu-id="7c6b1-143">Hier ist ein Beispiel für eine minimale Anforderung Anwendungsberechtigungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-143">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="7c6b1-144">Durch andere Eigenschaften auslassen, ist der Client implizit Standardwerte aus der vordefinierten Vorlage dargestellt durch Offlineschalten `template`.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-144">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="7c6b1-145">Wenn einer Anforderung mit Berechtigungen eines [Benutzers](../resources/user.md) ausstellen muss angegeben werden der `owners` Auflistung.</span><span class="sxs-lookup"><span data-stu-id="7c6b1-145">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="7c6b1-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6b1-146">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7c6b1-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6b1-147">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="7c6b1-148">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="7c6b1-148">See also</span></span>

- [<span data-ttu-id="7c6b1-149">Erstellen einer Gruppe mit einem team</span><span class="sxs-lookup"><span data-stu-id="7c6b1-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
