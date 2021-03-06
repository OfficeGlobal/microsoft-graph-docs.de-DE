---
title: team-Ressourcentyp
description: 'Ein Team in Microsoft Teams ist eine Sammlung von Kanälen. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9a5f1968753d3d2412b3885e6a09e94f18731e40
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458680"
---
# <a name="team-resource-type"></a>team-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Team in Microsoft Teams ist eine Sammlung von [Kanälen](channel.md). Ein Kanal stellt ein Thema und somit eine logische Trennung einer Unterhaltung in einem Team dar.

Jedes Team wird einer [Gruppe](../resources/group.md) zugeordnet.
Die Gruppe hat die gleiche ID wie das Team – z. B. ist /groups/{id}/team identisch mit /teams/{id}.
Weitere Informationen zum Arbeiten mit Gruppen und Mitgliedern in Teams finden Sie unter [Verwenden der Microsoft Graph REST-API zum Arbeiten mit Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Team erstellen](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Erstellen eines von Grund auf neuen Teams. |
|[Team aus Gruppe erstellen](../api/team-put-teams.md) | [team](team.md) | Erstellen eines neuen Teams oder Hinzufügen eines Teams zu einer vorhandenen Gruppe.|
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
|[Kanalnachrichten auflisten](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [Abrufen von Nachrichten in einem Kanal](../api/channel-list-messages.md) |
|[Kanalnachricht senden](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [Senden einer Nachricht an einen Kanal](../api/channel-post-chatmessage.md) |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|displayName|string| Der Name des Teams. |
|description|string| Eine optionale Beschreibung für das Team. |
|classification|string| Eine optionale Bezeichnung. Beschreibt in der Regel die Daten- oder Geschäftssensitivität des Teams. Muss mit einem der im Verzeichnis des Mandanten vorkonfigurierten Sätze übereinstimmen. |
|specialization|[teamSpecialization](teamspecialization.md)| Optional. Gibt an, ob das Team für einen bestimmten Anwendungsfall vorgesehen ist.  Jede Teamspezialisierung hat Zugriff auf eindeutige Verhaltensweisen und Oberflächen, die auf den Anwendungsfall zugeschnitten sind. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| Die Sichtbarkeit einer Gruppe und eines Teams. Der Standardwert ist „öffentlich“. |
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
|apps|[teamsApp](teamsapp.md)-Sammlung| (Veraltet) Die in diesem Team installierten Apps.|
|channels|[channel](channel.md)-Sammlung|Die Sammlung von Kanälen und Nachrichten, die mit dem Team verknüpft ist.|
|installedApps|[teamsAppInstallation](teamsappinstallation.md)-Sammlung|Die in diesem Team installierten Apps.|
|owners|[user](user.md)| Die Liste der Besitzer des Teams. Derzeit muss beim Erstellen eines Teams mit Anwendungsberechtigungen genau ein Besitzer angegeben werden. Bei Verwendung von benutzerdelegierten Berechtigungen kann kein Besitzer angegeben werden (der aktuelle Benutzer ist der Besitzer). Der Besitzer muss als Objekt-ID (GUID) und nicht als UPN angegeben werden. |
|operations|[teamsAsyncOperation](teamsasyncoperation.md)-Auflistung| Die asynchronen Vorgänge, die ausgeführt wurden oder in diesem Team ausgeführt werden. | 
|template|[teamsTemplate](teamstemplate.md)| Die Vorlage, von der dieses Team erstellt wurde. Siehe [Verfügbare Vorlagen](https://docs.microsoft.com/de-DE/MicrosoftTeams/get-started-with-teams-templates). |

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
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/team.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a>Siehe auch
- [Erstellen einer Gruppe mit einem Team](/graph/teams-create-group-and-team)
- [Übersicht über die Teams-API](teams-api-overview.md)
