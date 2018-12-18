---
title: Erstellen einer Gruppe mit einem Microsoft Teams-Team
description: 'Das Erstellen einer Gruppe, die ein Team umfasst, beinhaltet zwei Schritte: '
author: nkramer
ms.openlocfilehash: ea11d0ee7ee4e6e1d0bf6dc10ab8c9d064aa3610
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313888"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>Erstellen einer Gruppe mit einem Microsoft Teams-Team

Das Erstellen einer [Gruppe](/graph/api/resources/group?view=graph-rest-beta), die ein [Team](/graph/api/resources/team?view=graph-rest-beta) umfasst, beinhaltet zwei Schritte: 

- Das [Erstellen einer Gruppe](/graph/api/group-post-groups?view=graph-rest-beta) mit den richtigen Eigenschaften.
- Das [Hinzufügen eines Teams](/graph/api/team-put-teams?view=graph-rest-beta) zur Gruppe.

## <a name="create-a-group"></a>Erstellen einer Gruppe

Um ein Team einzuschließen, müssen Sie die folgenden Eigenschaftswerte festlegen, wie im folgenden Beispiel gezeigt:

- **groupTypes** = { "Unified" } 
- **mailEnabled** = true
- **securityEnabled** = false

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

Das folgende Beispiel zeigt die Antwort. 

>**Hinweis:** Das gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>Hinzufügen eines Teams zur Gruppe

Fügen Sie der Gruppe, wie dargestellt, ein Team hinzu.

```http
PUT /groups/{id}/team
{ }
```

Das folgende Beispiel zeigt die Antwort. 

>**Hinweis:** Das gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

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

Das erstellte Team hat die gleiche ID wie die Gruppe.
