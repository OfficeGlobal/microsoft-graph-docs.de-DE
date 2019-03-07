---
title: Team erstellen
description: Erstellt ein neues Team.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 394fa92f6ef97d6bc7a8dff0d4ddfe10c677bf99
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458687"
---
# <a name="create-team"></a>Team erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellt ein neues [Team](../resources/team.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| :------------------------------------- | :------------------------------------------ |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Group.ReadWrite.All                         |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                              |
| Anwendung                            | Group.ReadWrite.All                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile        | Wert                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung eines [team](../resources/team.md)-Objekts an.

## <a name="response"></a>Antwort

Falls erfolgreich, gibt diese API eine `202 Accepted`-Antwort mit einem Link zu [teamsAsyncOperation](../resources/teamsasyncoperation.md) zurück.

## <a name="examples"></a>Beispiele

### <a name="example-1-delegated-permissions"></a>Beispiel 1: Delegierte Berechtigungen

Nachfolgend sehen Sie ein Beispiel für eine Mindestanforderung. Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird.

#### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```

##### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-2-application-permissions"></a>Beispiel 2: Anwendungsberechtigungen

Im Folgenden sehen Sie ein Beispiel für eine Mindestanforderung unter Verwendung der Anwendungsberechtigungen. Durch Auslassen anderer Eigenschaften verwendet der Client implizit die Standardwerte aus der vordefinierten Vorlage, die durch `template` angegeben wird. Wenn Sie eine Anforderung mit Anwendungsberechtigungen erstellen, muss ein [Benutzer](../resources/user.md) in der `owners`-Sammlung angegeben werden.

#### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-3-create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a>Beispiel 3: Erstellen eines Teams mit einer App, mehreren Kanälen mit angehefteten Registerkarten unter Verwendung delegierter Berechtigungen

Im Folgenden sehen Sie eine Anforderung mit vollständiger Nutzlast. Der Client kann Werte in der Basisvorlage außer Kraft setzen und zu Elementen mit Arraywerten hinzufügen, soweit es die Validierungsregeln für `specialization` zulassen. 

#### <a name="request"></a>Anforderung

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

#### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-4-create-a-team-with-a-non-standard-base-template-type"></a>Beispiel 4: Erstellen eines Teams mit einem nicht standardmäßigen Basisvorlagentyp

Basisvorlagentypen sind spezielle Vorlagen, die Microsoft für bestimmte Branchen erstellt. Diese Basisvorlagen enthalten häufig proprietäre Apps, die nicht im Store verfügbar sind, und Teameigenschaften, die noch nicht separat in Microsoft Teams-Vorlagen unterstützt werden.

Um ein Team aus einer nicht standardmäßigen Basisvorlage zu erstellen, sollten Sie die `template@odata.bind`-Eigenschaft im Anforderungstext aus `standard` verwenden, um auf die spezifische Basisvorlage zu zeige, die Sie erstellen möchten.

Weitere Informationen zu unterstützten Basisvorlagentypen finden Sie unter [Erste Schritte mit Teams-Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).

#### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```

#### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example-5-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a>Beispiel 5: Erstellen eines Teams mit einem nicht standardmäßigen Basisvorlagentyp mit erweiterten Eigenschaften

Basisvorlagentypen können mit zusätzlichen Eigenschaften erweitert werden, sodass Sie auf einer vorhandenen Basisvorlage mit zusätzlichen Teameinstellungen, Kanälen, Apps oder Registerkarten aufbauen können.

Weitere Informationen zu unterstützten Basisvorlagentypen und erweiterten Eigenschaften finden Sie unter [Erste Schritte mit Teams-Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates).

#### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
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

#### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a>Siehe auch

- [Verfügbare Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates)
- [Erste Schritte mit Vorlagen für Teams im Einzelhandel](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [Erste Schritte mit Vorlagen für Teams im Gesundheitswesen](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [Erstellen einer Gruppe mit einem Team](/graph/teams-create-group-and-team)

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/api/team-post.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
