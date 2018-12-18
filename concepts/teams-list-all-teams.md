---
title: Auflisten aller Teams einer Organisation in Microsoft Teams
description: 'Auflisten aller Teams '
author: nkramer
ms.openlocfilehash: f8f088dd9b7a55d3eb4c927ddef34458caeab507
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304159"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>Auflisten aller Teams einer Organisation in Microsoft Teams

Um alle [Teams](/graph/api/resources/team?view=graph-rest-beta) in einer Organisation (einem Mandanten) aufzulisten, suchen Sie alle Gruppen, die über Teams verfügen und rufen dann Informationen für jedes Team ab.

## <a name="get-a-list-of-groups"></a>Abrufen einer Liste von Gruppen

Um eine Liste aller [Gruppen](/graph/api/resources/group?view=graph-rest-beta) in der Organisation abzurufen, die über Teams verfügen, rufen Sie eine [Liste aller Gruppen](/graph/api/group-list?view=graph-rest-beta) ab, und suchen Sie dann im Code diejenigen Gruppen, deren Eigenschaft **resourceProvisioningOptions** "Team" enthält.
Da es sich bei Gruppen um große Objekte handelt, verwenden Sie "$select", um nur die Eigenschaften der in Frage kommenden Gruppe abzurufen.

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> **Hinweis**: Bei einigen nicht verwendeten alten Teams ist die Eigenschaft "resourceProvisioningOptions" nicht festgelegt. Einzelheiten hierzu finden Sie unter [bekannte Probleme](known-issues.md#missing-teams-in-list-all-teams).

Nachfolgend sehen Sie ein Beispiel der Antwort. 

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

## <a name="get-a-list-of-groups-using-beta-apis"></a>Abrufen einer Liste der Gruppen mit Beta-APIs

Mithilfe der Beta-APIs können Sie "$filter" verwenden, um nur die Gruppen zurückzugeben, die über Teams verfügen.

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> **Hinweis**: "$filter" ist für "/groups" nur über den Beta-Endpunkt verfügbar. "resourceProvisioningOptions" ist in v1.0 und in der Beta verfügbar.

> **Hinweis**: Bestimmte nicht verwendete alte Teams werden nicht aufgelistet. Einzelheiten hierzu finden Sie unter [bekannte Probleme](known-issues.md#missing-teams-in-list-all-teams).

Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

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

## <a name="get-team-information-for-a-group"></a>Abrufen von Teaminformationen für eine Gruppe

Um Teaminformationen für das Team in einer bestimmten Gruppe abzurufen, rufen Sie die [get team](/graph/api/team-get?view=graph-rest-beta)-API auf, und schließen Sie die Gruppen-ID ein.

```http
GET /teams/{group-id}
```

Das folgende Beispiel zeigt die Antwort.

>**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
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

## <a name="see-also"></a>Siehe auch

- [joinedTeams auflisten](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [Gruppen auflisten](/graph/api/group-list?view=graph-rest-beta)
