---
title: Team erstellen
description: Erstellt ein neues Team.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d5463bdc2cc5aa5b471e9526be579364991645ad
ms.sourcegitcommit: 597dfc95a44e0f2354d056b5567bcff2bb2837f1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29892519"
---
# <a name="create-team"></a><span data-ttu-id="53fbc-103">Team erstellen</span><span class="sxs-lookup"><span data-stu-id="53fbc-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53fbc-104">Erstellt ein neues [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="53fbc-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53fbc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53fbc-105">Permissions</span></span>

<span data-ttu-id="53fbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53fbc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53fbc-108">Permission type</span></span>                        | <span data-ttu-id="53fbc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53fbc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="53fbc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53fbc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53fbc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53fbc-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="53fbc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53fbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53fbc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53fbc-113">Not supported.</span></span>                              |
| <span data-ttu-id="53fbc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53fbc-114">Application</span></span>                            | <span data-ttu-id="53fbc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53fbc-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="53fbc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="53fbc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53fbc-117">Request headers</span></span>

| <span data-ttu-id="53fbc-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53fbc-118">Header</span></span>        | <span data-ttu-id="53fbc-119">Wert</span><span class="sxs-lookup"><span data-stu-id="53fbc-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="53fbc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53fbc-120">Authorization</span></span> | <span data-ttu-id="53fbc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53fbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53fbc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53fbc-123">Content-Type</span></span>  | <span data-ttu-id="53fbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53fbc-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="53fbc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53fbc-125">Request body</span></span>

<span data-ttu-id="53fbc-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [team](../resources/team.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="53fbc-126">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53fbc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-127">Response</span></span>

<span data-ttu-id="53fbc-128">Falls erfolgreich, gibt diese API eine `202 Accepted`-Antwort mit einem Link zu [teamsAsyncOperation](../resources/teamsasyncoperation.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="53fbc-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="53fbc-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="53fbc-129">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="53fbc-130">Beispiel 1: Delegierte Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53fbc-130">Example 1: Delegated permissions</span></span>

<span data-ttu-id="53fbc-131">Nachfolgend sehen Sie ein Beispiel für eine Mindestanforderung.</span><span class="sxs-lookup"><span data-stu-id="53fbc-131">The following is an example of a minimal request.</span></span> <span data-ttu-id="53fbc-132">Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="53fbc-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="53fbc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a><span data-ttu-id="53fbc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="53fbc-135">Beispiel 2: Anwendungsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="53fbc-135">Example 2: Application permissions</span></span>

<span data-ttu-id="53fbc-136">Im Folgenden sehen Sie ein Beispiel für eine Mindestanforderung unter Verwendung der Anwendungsberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="53fbc-136">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="53fbc-137">Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="53fbc-137">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="53fbc-138">Wenn Sie eine Anforderung mit Anwendungsberechtigungen erstellen, muss ein [Benutzer](../resources/user.md) in der `owners`-Sammlung angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="53fbc-138">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="53fbc-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-139">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="53fbc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-140">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-3-create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="53fbc-141">Beispiel 3: Erstellen eines Teams mit einer App, mehreren Kanälen mit angehefteten Registerkarten unter Verwendung delegierter Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53fbc-141">Example 3: Create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="53fbc-142">Im Folgenden sehen Sie eine Anforderung mit vollständiger Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="53fbc-142">The following is a request with a full payload.</span></span> <span data-ttu-id="53fbc-143">Der Client kann Werte in der Basisvorlage außer Kraft setzen und zu Elementen mit Arraywerten hinzufügen, soweit es die Validierungsregeln für `specialization` zulassen.</span><span class="sxs-lookup"><span data-stu-id="53fbc-143">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span> 

#### <a name="request"></a><span data-ttu-id="53fbc-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
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

#### <a name="response"></a><span data-ttu-id="53fbc-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-4-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="53fbc-146">Beispiel 4: Erstellen eines Teams mit einem nicht standardmäßigen Basisvorlagentyp</span><span class="sxs-lookup"><span data-stu-id="53fbc-146">Example 4: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="53fbc-147">Basisvorlagentypen sind spezielle Vorlagen, die Microsoft für bestimmte Branchen erstellt.</span><span class="sxs-lookup"><span data-stu-id="53fbc-147">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="53fbc-148">Diese Basisvorlagen enthalten häufig proprietäre Apps, die nicht im Store verfügbar sind, und Teameigenschaften, die noch nicht separat in Microsoft Teams-Vorlagen unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="53fbc-148">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="53fbc-149">Um ein Team aus einer nicht standardmäßigen Basisvorlage zu erstellen, sollten Sie die `template@odata.bind`-Eigenschaft im Anforderungstext aus `standard` verwenden, um auf die spezifische Basisvorlage zu zeige, die Sie erstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="53fbc-149">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="53fbc-150">Weitere Informationen zu unterstützten Basisvorlagentypen finden Sie unter [Erste Schritte mit Teams-Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="53fbc-150">To learn more about supported base template types, see [Get started with Teams templates](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="53fbc-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-151">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/educationClass",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a><span data-ttu-id="53fbc-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-152">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-5-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="53fbc-153">Beispiel 5: Erstellen eines Teams mit einem nicht standardmäßigen Basisvorlagentyp mit erweiterten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53fbc-153">Example 5: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="53fbc-154">Basisvorlagentypen können mit zusätzlichen Eigenschaften erweitert werden, sodass Sie auf einer vorhandenen Basisvorlage mit zusätzlichen Teameinstellungen, Kanälen, Apps oder Registerkarten aufbauen können.</span><span class="sxs-lookup"><span data-stu-id="53fbc-154">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="53fbc-155">Weitere Informationen zu unterstützten Basisvorlagentypen und erweiterten Eigenschaften finden Sie unter [Erste Schritte mit Teams-Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).</span><span class="sxs-lookup"><span data-stu-id="53fbc-155">To learn more about supported base template types and supported properties, see [Get started with Teams templates](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="53fbc-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53fbc-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/educationClass",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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

#### <a name="response"></a><span data-ttu-id="53fbc-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="53fbc-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="53fbc-158">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="53fbc-158">See also</span></span>

- [<span data-ttu-id="53fbc-159">Verfügbare Vorlagen</span><span class="sxs-lookup"><span data-stu-id="53fbc-159">Available templates</span></span>](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates)
- [<span data-ttu-id="53fbc-160">Erste Schritte mit Vorlagen für Teams im Einzelhandel</span><span class="sxs-lookup"><span data-stu-id="53fbc-160">Getting started with Retail Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [<span data-ttu-id="53fbc-161">Erste Schritte mit Vorlagen für Teams im Gesundheitswesen</span><span class="sxs-lookup"><span data-stu-id="53fbc-161">Getting started with Healthcare Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [<span data-ttu-id="53fbc-162">Erstellen einer Gruppe mit einem Team</span><span class="sxs-lookup"><span data-stu-id="53fbc-162">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/api/team-post.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
