---
title: team-Ressourcentyp
description: 'Ein Team in Microsoft Teams ist eine Sammlung von Kanälen. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 692f0d12c172fb6b7088912eec952b519d852cac
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735572"
---
# <a name="team-resource-type"></a>team-Ressourcentyp



Ein Team in Microsoft Teams ist eine Sammlung von [Kanälen](channel.md). Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.

Jedes Team wird einer [Gruppe](../resources/group.md) zugeordnet.
Die Gruppe hat die gleiche ID wie das Team – z. B. ist /groups/{id}/team identisch mit /teams/{id}.
Weitere Informationen zum Arbeiten mit Gruppen und Mitgliedern in Teams finden Sie unter [Verwenden der Microsoft Graph REST-API zum Arbeiten mit Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Team erstellen](../api/team-put-teams.md) | [team](team.md) | Erstellen eines neuen Teams oder Hinzufügen eines Teams zu einer vorhandenen Gruppe.|
|[Team abrufen](../api/team-get.md) | [team](team.md) | Abrufen der Eigenschaften und Beziehungen des angegebenen Teams.|
|[Team aktualisieren](../api/team-update.md) | [team](team.md) |Aktualisieren der Eigenschaften des angegebenen Teams. |
|[Team löschen](/graph/api/group-delete?view=graph-rest-1.0) | Keine |Löschen des Teams und der zugehörigen Gruppe. |
|[Team klonen](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Kopieren des Teams und der zugehörigen Gruppe. |
|[Team archivieren](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Versetzen des Teams in einen schreibgeschützten Zustand. |
|[Archivierung von Team aufheben](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Zurückversetzen des Teams in den Zustand Lesen/Schreiben. |
|[Ihre Teams auflisten](../api/user-list-joinedteams.md) | [team](team.md)-Sammlung | Auflisten der Teams, in denen Sie Mitglied sind. |
|[Auflisten aller Teams](/graph/teams-list-all-teams) | [group](group.md)-Sammlung | Auflisten aller Gruppen, die über Teams verfügen. |
|[Apps in Ihrer Organisation veröffentlichen](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Erstellen von Teams-Apps, die nur für Ihre Organisation sichtbar sind. |
|[App zu Team hinzufügen](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | Hinzufügen (Installieren) einer App zu einem Team.|
|[Registerkarte zu Kanal hinzufügen](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | Hinzufügen (Installieren) einer Registerkarte zum Kanal des Teams.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|funSettings|[teamFunSettings](teamfunsettings.md) |Einstellungen zum Konfigurieren der Verwendung von Giphy, Memen und Aufklebern im Team.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Einstellungen zum Konfigurieren, ob Gäste Kanäle im Team erstellen, aktualisieren oder löschen können.|
|internalId | Zeichenfolge | Eine eindeutige ID für das Team, das an einigen Stellen verwendet wurde, zum Beispiel Überwachungsprotokoll/[Office 365-Verwaltungsaktivitäts-API](https://docs.microsoft.com/de-DE/office/office-365-management-api/office-365-management-activity-api-reference). |
|isArchived|Boolesch|Gibt an, ob sich das Team im schreibgeschützten Modus befindet. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Einstellungen zum Konfigurieren, ob Mitglieder bestimmte Aktionen, z. B. Kanäle erstellen und Bots hinzufügen, im Team ausführen können.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Einstellungen zum Konfigurieren von Messaging und Erwähnungen im Team.|
|webUrl|string (schreibgeschützt) | Ein Link, der im Microsoft Teams-Client zu dem Team führt. Dies ist die URL, die Sie erhalten, wenn Sie im Microsoft Teams-Client mit der rechten Maustaste auf ein Team klicken und **Link zum Team abrufen** auswählen. Diese URL sollte als nicht transparenter Blob behandelt und nicht analysiert werden. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|channels|[channel](channel.md)-Sammlung|Die Sammlung von Kanälen und Nachrichten, die mit dem Team verknüpft ist.|
|installedApps|[teamsAppInstallation](teamsappinstallation.md)-Sammlung|Die in diesem Team installierten Apps.|

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
  "internalId": "19:...big.number...@thread.skype",
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
- [Erstellen einer Gruppe mit einem Team](/graph/teams-create-group-and-team)
- [Verwenden der Teams-API](teams-api-overview.md)
