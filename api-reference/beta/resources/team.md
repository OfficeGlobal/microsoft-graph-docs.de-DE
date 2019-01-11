---
title: Team Ressourcentyp
description: 'Ein Team in Microsoft-Teams ist eine Auflistung der Kanäle. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: bf76f7b4b6cd06afb80b17e82fb8d10675b744a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862263"
---
# <a name="team-resource-type"></a>Team Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Team in Microsoft-Teams ist eine Auflistung der [Kanäle](channel.md). Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.

Jedes Team ist eine [Gruppe](../resources/group.md)zugeordnet.
Die Gruppe verfügt über die gleiche ID wie die Team - beispielsweise /groups/ {Id} / Team ist identisch mit /teams/ {Id}.
Weitere Informationen über das Arbeiten mit Gruppen und Membern im Teams finden Sie unter [Verwenden der Microsoft Graph-REST-API entwickelt Microsoft-Teams](teams-api-overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von Teams](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Erstellen Sie ein Team von Grund auf neu. |
|[Erstellen von Teams aus Gruppe](../api/team-put-teams.md) | [Team](team.md) | Erstellen Sie ein neues Team oder fügen Sie ein Team an eine vorhandene Gruppe hinzu.|
|[Get-team](../api/team-get.md) | [Team](team.md) | Abrufen der Eigenschaften und Beziehungen zwischen dem angegebenen Team.|
|[Update-team](../api/team-update.md) | [Team](team.md) |Aktualisieren Sie die Eigenschaften des angegebenen Teams. |
|[Team löschen](/graph/api/group-delete?view=graph-rest-1.0) | Keine |Das Team und der zugeordneten Gruppe zu löschen. |
|[Wenn Sie den Klon-team](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Kopieren Sie das Team und dessen zugehörige Gruppe. |
|[Archiv-team](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Platzieren Sie das Team in einem schreibgeschützten Zustand. |
|[Entpackt team](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Wiederherstellen Sie das Team eine Lese-/ Schreibzugriff Zustand. |
|[Listen Sie Ihren teams](../api/user-list-joinedteams.md) | [Team](team.md) -Auflistung | Listen Sie Teams, denen Sie Mitglied sind. |
|[Listen Sie alle teams](/graph/teams-list-all-teams) | [Gruppensammlung](group.md) | Listen Sie alle Gruppen, bei die Teams haben. |
|[Veröffentlichen von apps in Ihrer Organisation](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Erstellen von Teams apps wird nur für Ihre Organisation angezeigt. |
|[Team app hinzufügen](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | Fügt (installiert) einer app zu einem Team.|
|[Registerkarte Channel hinzufügen](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | Fügt (installiert) eine Registerkarte, um ein Team des DDE-Kanal.|
|[Liste Channel Nachrichten](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [Abrufen von Nachrichten in einem Kanal](../api/channel-list-messages.md) |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|displayName|string| Der Name des Teams. |
|description|string| Eine optionale Beschreibung für das Team. |
|Klassifikation|string| Eine optionale Bezeichnung. In der Regel werden die Daten oder Business Vertraulichkeit des Teams beschrieben. Dabei muss es sich um eine Reihe vorkonfigurierten im Verzeichnis für den Mandanten übereinstimmen. |
|Spezialisierung|[teamSpecialization](teamspecialization.md)| Optional. Gibt an, ob das Team für einen bestimmten Anwendungsfall vorgesehen ist.  Jedes Team Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| Der Sichtbarkeit von einer Gruppe und Team. Der Standardwert ist öffentlich. |
|funSettings|[teamFunSettings](teamfunsettings.md) |So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.|
|isArchived|Boolean|Gibt an, ob dieses Team im schreibgeschützten Modus ist. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.|
|webUrl|Zeichenfolge (schreibgeschützt) | Ein Hyperlink, der an das Team in der Microsoft-Teams, Client gesendet wird. Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten ein Team in der Microsoft-Teams, Client Maustaste und wählen Sie **Link an das Team abrufen**. Diese URL sollte als nicht transparentes Blob behandelt und nicht analysiert werden. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|Apps|[TeamsApp](teamsapp.md) -Auflistung| (Veraltet) Die apps in dieser Gruppe installiert.|
|Kanäle|[Kanal](channel.md) -Auflistung|Die Auflistung der Kanäle & Nachrichten, die dem Team zugeordnet.|
|installedApps|[TeamsAppInstallation](teamsappinstallation.md) -Auflistung|Die apps in dieser Gruppe installiert.|
|owners|[Benutzer](user.md)| Die Liste der Besitzer des Teams. |
|template|[teamsTemplate](teamstemplate.md)| Die Vorlage wurde dieses Team aus erstellt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Siehe auch
- [Erstellen einer Gruppe mit einem team](/graph/teams-create-group-and-team)
- [Teams-API (Übersicht)](teams-api-overview.md)
