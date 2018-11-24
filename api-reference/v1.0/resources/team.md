# <a name="team-resource-type"></a>Team Ressourcentyp



Ein Team in Microsoft-Teams ist eine Auflistung der [Kanäle](channel.md). Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams.

Jedes Team ist eine [Gruppe](../resources/group.md)zugeordnet.
Die Gruppe verfügt über die gleiche ID wie die Team - beispielsweise /groups/ {Id} / Team ist identisch mit /teams/ {Id}.
Weitere Informationen über das Arbeiten mit Gruppen und Membern im Teams finden Sie unter [Verwenden der Microsoft Graph-REST-API entwickelt Microsoft-Teams](teams_api_overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von Teams](../api/team_put_teams.md) | [Team](team.md) | Erstellen Sie ein neues Team oder fügen Sie ein Team an eine vorhandene Gruppe hinzu.|
|[Get-team](../api/team_get.md) | [Team](team.md) | Abrufen der Eigenschaften und Beziehungen zwischen dem angegebenen Team.|
|[Update-team](../api/team_update.md) | [Team](team.md) |Aktualisieren Sie die Eigenschaften des angegebenen Teams. |
|[Team löschen](../../v1.0/api/group_delete.md) | Keine |Das Team und der zugeordneten Gruppe zu löschen. |
|[Wenn Sie den Klon-team](../api/team_clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Kopieren Sie das Team und dessen zugehörige Gruppe. |
|[Archiv-team](../api/team_archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Platzieren Sie das Team in einem schreibgeschützten Zustand. |
|[Entpackt team](../api/team_unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Wiederherstellen Sie das Team eine Lese-/ Schreibzugriff Zustand. |
|[Listen Sie Ihren teams](../api/user_list_joinedteams.md) | [Team](team.md) -Auflistung | Listen Sie Teams, denen Sie Mitglied sind. |
|[Listen Sie alle teams](../../../concepts/teams_list_all_teams.md) | [Gruppensammlung](group.md) | Listen Sie alle Gruppen, bei die Teams haben. |
|[Veröffentlichen von apps in Ihrer Organisation](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Erstellen von Teams apps wird nur für Ihre Organisation angezeigt. |
|[Team app hinzufügen](../api/teamsappinstallation_add.md) | [teamsappinstallation](teamsappinstallation.md) | Fügt (installiert) einer app zu einem Team.|
|[Registerkarte Channel hinzufügen](../api/teamstab_add.md) | [teamsTab](../resources/teamstab.md) | Fügt (installiert) eine Registerkarte, um ein Team des DDE-Kanal.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|funSettings|[teamFunSettings](teamfunsettings.md) |So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.|
|isArchived|Boolescher Wert|Gibt an, ob dieses Team im schreibgeschützten Modus ist. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.|
|webUrl|Zeichenfolge (schreibgeschützt) | Ein Hyperlink, der an das Team in der Microsoft-Teams, Client gesendet wird. Dies ist die URL, die Sie erhalten, wenn Sie mit der rechten ein Team in der Microsoft-Teams, Client Maustaste und wählen Sie **Link an das Team abrufen**. Diese URL sollte als nicht transparentes Blob behandelt und nicht analysiert werden. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|Kanäle|[Kanal](channel.md) -Auflistung|Die Auflistung der Kanäle & Nachrichten, die dem Team zugeordnet.|
|installedApps|[TeamsAppInstallation](teamsappinstallation.md) -Auflistung|Die apps in dieser Gruppe installiert.|

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
- [Erstellen einer Gruppe mit einem team](../../../concepts/teams-create-group-and-team.md)
- [Verwenden von Teams-APIs](teams_api_overview.md)
