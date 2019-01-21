---
title: Gruppen-Ressourcentyp
description: Stellt eine Azure Active Directory (Azure AD)-Gruppe dar, bei der es sich um eine Office 365-Gruppe, ein Team in Microsoft Teams, eine dynamische Gruppe oder eine Sicherheitsgruppe handeln kann.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: b9f4e249c763b7617e946432d10f33166173dd84
ms.sourcegitcommit: d9d8b908061b3680e8a52790a6c9aaf8e51ceea0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/17/2019
ms.locfileid: "28328013"
---
# <a name="group-resource-type"></a>Gruppen-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Azure Active Directory (Azure AD)-Gruppe dar, bei der es sich um eine Office 365-Gruppe, ein Team in Microsoft Teams, eine dynamische Gruppe oder eine Sicherheitsgruppe handeln kann.
Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften als [Erweiterungen](/graph/extensibility-overview).
- Abonnieren von [Änderungsbenachrichtigungen](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user-delta.md)-Funktion.

> **Microsoft Teams- und Office 365-Gruppen unterstützen Gruppenzusammenarbeit**. Der Großteil der Office 365-Gruppen-API kann mit Microsoft Teams verwendet werden. Um ein [Team](team.md) zu erstellen, müssen Sie zuerst eine [Gruppe erstellen](../api/group-post-groups.md) und dann [ein Team zur Gruppe hinzufügen](../api/team-put-teams.md). Weitere Informationen finden Sie in der [Übersicht über Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|**Gruppenverwaltung**| | |
|[Gruppe erstellen](../api/group-post-groups.md) | [group](group.md) |Erstellt eine neue Gruppe gemäß den Angaben. Dabei kann es sich um eine Office 365-Gruppe, eine dynamische Gruppe, eine Sicherheitsgruppe oder ein Team handeln.|
|[Gruppe abrufen](../api/group-get.md) | [group](group.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des group-Objekts.|
|[Gruppe aktualisieren](../api/group-update.md) | Keine |Aktualisiert die Eigenschaften eines Gruppenobjekts. |
|[Gruppe löschen](../api/group-delete.md) | Keiner |Löscht das Gruppenobjekt. |
|[delta](../api/group-delta.md)|group-Sammlung| Dient zum Abrufen inkrementeller Änderungen für Gruppen. |
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung| Dient zum Auflisten der Gruppenlebenszyklusrichtlinien. |
|[Besitzer auflisten](../api/group-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Besitzer der Gruppe aus der **owners**-Navigationseigenschaft ab.|
|[Besitzer hinzufügen](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| Fügt einen neuen Besitzer zur Gruppe durch Bereitstellen an die **owners**-Navigationseigenschaft hinzu (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Besitzer entfernen](../api/group-delete-owners.md) | Keiner |Entfernt einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe über die **owners**-Navigationseigenschaft.|
|[Mitglieder auflisten](../api/group-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer und Gruppen, die direkte Mitglieder dieser Gruppe sind, aus der **members**-Navigationseigenschaft ab.|
|[Transitive Mitglieder auflisten](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer, Gruppen, Geräte und Dienstprinzipale ab, die Mitglieder sind, einschließlich der geschachtelten Mitglieder dieser Gruppe.|
|[Mitglied hinzufügen](../api/group-post-members.md) |[directoryObject](directoryobject.md)| Fügt dieser Gruppe einen Benutzer oder eine Gruppe durch Bereitstellung an die **members**-Navigationseigenschaft hinzu (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Mitglied entfernen](../api/group-delete-members.md) | Keine |Entfernt ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe anhand der **members**-Navigationseigenschaft. Sie können Benutzer oder andere Gruppen entfernen. |
|[memberOf auflisten](../api/group-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Gruppen und administrativen Einheiten, in denen diese Gruppe ein direktes Mitglied ist, aus der memberOf-Navigationseigenschaft ab.|
|[Transitive memberOf auflisten](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Listet die Gruppen und administrativen Einheiten auf, bei denen der Benutzer Mitglied ist. Dieser Vorgang ist transitiv und schließt die Gruppen ein, in denen diese Gruppe ein geschachteltes Mitglied. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Zeichenfolgenauflistung|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Funktion ist transitiv.|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist. Die Funktion ist transitiv.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Zeichenfolgenauflistung|Gibt alle Gruppen und administrativen Einheiten zurück, in denen der Benutzer Mitglied ist. Die Funktion ist transitiv. |
|[Einstellung erstellen](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Erstellt ein Einstellungsobjekt basierend auf einer directorySettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen angeben, die in der Vorlage definiert sind. Für diesen Vorgang können nur gruppenspezifische Vorlagen verwendet werden.|
|[Einstellung abrufen](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.|
|[Einstellungen auflisten](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) collection |Listet Eigenschaften aller Einstellungsobjekte auf.|
|[Einstellung aktualisieren](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Aktualisiert ein Einstellungsobjekt. |
|[Einstellung löschen](../api/directorysetting-delete.md) | Keine |Löscht ein Einstellungsobjekt. |
|[Endpunkte auflisten](../api/group-list-endpoints.md) |[endpoint](endpoint.md)-Sammlung| Ruft eine Endpunktobjektsammlung ab. |
|[Endpunkt abrufen](../api/endpoint-get.md) | [endpoint](endpoint.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des endpoint-Objekts. |
|[delta](../api/group-delta.md)|group-Sammlung| Ruft inkrementelle Änderungen für Gruppen ab. |
|[validateProperties](../api/group-validateproperties.md)|JSON| Überprüft, ob der Anzeigename oder E-Mail-Kontoname einer Office 365-Gruppe den Benennungsrichtlinien entspricht. | 
|**Calendar**| | |
|[Ereignis erstellen](../api/group-post-events.md) |[Ereignis](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Ereignissammlung.|
|[Ereignis abrufen](../api/group-get-event.md) |[Ereignis](event.md)|Liest die Eigenschaften eines Ereignisobjekts.|
|[Ereignisse auflisten](../api/group-list-events.md) |[Ereignissammlung](event.md)| Ruft eine Ereignisobjektsammlung ab.|
|[Ereignis aktualisieren](../api/group-update-event.md) |Keine|Dient zum Aktualisieren der Eigenschaften eines Ereignisobjekts.|
|[Ereignis löschen](../api/group-delete-event.md) |Keine|Löscht das Ereignisobjekt.|
|[calendarView auflisten](../api/group-list-calendarview.md) |[Ereignissammlung](event.md)| Ruft eine Auflistung der Ereignisse in einem angegebenen Zeitfenster ab.|
|**Unterhaltungen**| | |
|[Unterhaltung erstellen](../api/group-post-conversations.md) |[Unterhaltung](conversation.md)| Erstellt eine neue Unterhaltung durch Veröffentlichung in der Unterhaltungssammlung.|
|[Unterhaltung abrufen](../api/group-get-conversation.md) |[Unterhaltung](conversation.md)| Dient zum Lesen der Eigenschaften eines Unterhaltungsobjekts.|
|[Unterhaltungen auflisten](../api/group-list-conversations.md) |[Unterhaltungssammlung](conversation.md)| Ruft eine Unterhaltungsobjektsammlung ab.|
|[Unterhaltung löschen](../api/group-delete-conversation.md) |Keine|Löscht ein Unterhaltungsobjekt.|
|[Thread abrufen](../api/group-get-thread.md) |[conversationThread](conversationthread.md)| Liest die Eigenschaften eines Threadobjekts.|
|[Threads auflisten](../api/group-list-threads.md) |[conversationThread](conversationthread.md)-Sammlung| Ruft alle Threads einer Gruppe ab.|
|[Thread aktualisieren](../api/group-update-thread.md) |Keine| Aktualisiert die Eigenschaften eines Threadobjekts.|
|[Thread löschen](../api/group-delete-thread.md) |Keine| Löscht das Threadobjekt.
|[acceptedSenders auflisten](../api/group-list-acceptedsenders.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der acceptedSenders für diese Gruppe befinden.|
|[acceptedSender hinzufügen](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Fügt einen Benutzer oder eine Gruppe zur acceptSenders-Sammlung hinzu.|
|[acceptedSender entfernen](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Entfernt einen Benutzer oder eine Gruppe aus der acceptedSenders-Sammlung.|
|[rejectedSenders auflisten](../api/group-list-rejectedsenders.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.|
|[rejectedSender hinzufügen](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Sammlung hinzu.|
|[rejectedSender entfernen](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Entfernt einen neuen Benutzer oder eine neue Gruppe aus der rejectedSenders-Sammlung.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Andere Gruppenressourcen**| | |
|[Fotos auflisten](../api/group-list-photos.md) |[profilePhoto](photo.md)-Sammlung| Ruft eine Sammlung von Profilfotos für die Gruppe ab.|
|[plannerPlans auflisten](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md)-Sammlung| Ruft Plannerer-Pläne im Besitz der Gruppe ab.|
|**Benutzereinstellungen**| | |
|[addFavorite](../api/group-addfavorite.md)|Keine|Fügt die Gruppe zu der Liste der Favoritengruppen des aktuellen Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.|
|[removeFavorite](../api/group-removefavorite.md)|Keine|Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.|
|[memberOf auflisten](../api/group-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Gruppen und administrativen Einheiten, bei denen dieser Benutzer direktes Mitglied ist, aus der **memberOf**-Navigationseigenschaft ab.|
|[joinedTeams auflisten](../api/user-list-joinedteams.md) |[group](group.md)-Sammlung| Ruft die Microsoft-Teams an, in denen der Benutzer ein direktes Mitglied ist.|
|[subscribeByMail](../api/group-subscribebymail.md)|Keiner|Legt die Eigenschaft „IsSubscribedByMail“ auf **true** fest. Aktiviert den aktuellen Benutzer für den Erhalt von E-Mail-Unterhaltungen. Wird nur für Office 365-Gruppen unterstützt.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Keiner|Legt die Eigenschaft „isSubscribedByMail“ auf **false** fest. Deaktiviert den aktuellen Benutzer für den Erhalt von E-Mail-Unterhaltungen. Wird nur für Office 365-Gruppen unterstützt.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Keiner|Setzt das unseenCount-Element aller Beiträge, die der aktuelle Benutzer seit dem letzten Besuch noch nicht gesehen hat, auf 0 zurück. Wird nur für Office 365-Gruppen unterstützt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolescher Wert|Der Standardwert ist **false**. Gibt an, ob Personen außerhalb der Organisation Nachrichten an die Gruppe senden können.|
|assignedLicenses|[assignedLicense](assignedlicense.md)-Sammlung|Die Lizenzen, die der Gruppe zugewiesen sind. Schreibgeschützt.|
|autoSubscribeNewMembers|Boolean|Der Standardwert ist **false**. Gibt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten. Sie können diese Eigenschaft in einer PATCH-Anforderung für die Gruppe festlegen; legen Sie sie nicht in der anfänglichen POST-Anforderung fest, mit der die Gruppe erstellt wird.|
|Klassifikation|Zeichenfolge|Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrige, mittlere oder hohe geschäftliche Auswirkungen). Gültige Werte für diese Eigenschaft werden durch die Erstellung eines ClassificationList-[setting](directorysetting.md)-Werts basierend auf der [Vorlagendefinition](directorysettingtemplate.md) erstellt.|
|createdDateTime|DateTimeOffset| Zeitstempel der Gruppenerstellung. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Gruppe erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|description|String|Eine optionale Beschreibung für die Gruppe.|
|displayName|String|Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.|
|expirationDateTime|DateTimeOffset| Zeitstempel des festgelegten Ablaufs der Gruppe. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Gruppe erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|groupTypes|Zeichenfolgenauflistung| Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind `Unified` zum Erstellen einer Office 365-Gruppe oder `DynamicMembership` für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-fähige Sicherheitsgruppen diese Eigenschaft nicht fest.|
|id|String|Eindeutiger Bezeichner für die Gruppe. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|isSubscribedByMail|Boolean|Der Standardwert ist **true**. Gibt an, ob der aktuelle Benutzer den Erhalt von E-Mail-Unterhaltungen abonniert hat.|
|licenseProcessingState|Zeichenfolge|Gibt den Status der Gruppenlizenzzuweisung an alle Mitglieder der Gruppe an. Schreibgeschützt. Mögliche Werte: `QueuedForProcessing`, `ProcessingInProgress` und `ProcessingComplete`.|
|mail|String|Die SMTP-Adresse für die Gruppe ein, z. B. „serviceadmins@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailEnabled|Boolean|Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.|
|mailNickname|String|Der E-Mail-Alias für die Gruppe (eindeutig in der Organisation). Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.|
|membershipRule|Zeichenfolge|Die Regel, die Mitglieder dieser Gruppe bestimmt, wenn die Gruppe eine dynamische Gruppe ist (enthält `DynamicMembership`). Weitere Informationen zur Syntax der Mitgliedschaftsregel finden Sie unter [Regeln für eine dynamische Mitgliedschaft](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|Zeichenfolge|Gibt an, ob die Verarbeitung der dynamischen Mitgliedschaft aktiv ist oder angehalten wurde. Mögliche Werte sind „On“ oder „Paused“.|
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis an. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. Unterstützt $filter.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)-Sammlung| Fehler bei Verwendung eines Microsoft-Synchronisierungsprodukts während der Bereitstellung. |
|onPremisesSecurityIdentifier|String|Enthält die lokale Sicherheits-ID (SID) für die Gruppe, die von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt. |
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt. Unterstützt $filter.|
|preferredDataLocation|Zeichenfolge|Der bevorzugte Datenspeicherort für die Gruppe. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für eine Office 365-Gruppe. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|proxyAddresses|Zeichenfolgenauflistung| Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Schreibgeschützt. Lässt keine NULL-Werte zu. Unterstützt $filter. |
|renewedDateTime|DateTimeOffset| Zeitstempel der letzten Verlängerung der Gruppe. Dies kann nicht direkt geändert werden und wird nur über die [Aktion zum Verlängern des Diensts](../api/grouplifecyclepolicy-renewgroup.md) aktualisiert. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|securityEnabled|Boolean|Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.|
|theme|Zeichenfolge|Gibt das Farbdesign einer Office 365-Gruppe an. Mögliche Werte sind `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` oder `Red`.|
|unseenConversationsCount|Int32|Die Anzahl von Unterhaltungen, an die seit dem letzten Besuch des angemeldeten Benutzers bei der Gruppe ein oder mehrere neue Beiträge übermittelt wurden. Diese Eigenschaft ist identisch mit **unseenCount**.|
|unseenCount|Int32|Die Anzahl von Unterhaltungen, an die seit dem letzten Besuch des angemeldeten Benutzers bei der Gruppe ein oder mehrere neue Beiträge übermittelt wurden. Diese Eigenschaft ist identisch mit **unseenConversationsCount**.|
|unseenMessagesCount|Int32|Die Anzahl neuer Beiträge, die seit dem letzten Besuch des angemeldeten Benutzers bei der Gruppe an die Unterhaltungen der Gruppe übermittelt wurden.|
|visibility|Zeichenfolge| Gibt die Sichtbarkeit einer Office 365-Gruppe an. Mögliche Werte sind: `private`, `public` oder `hiddenmembership`; leere Werte werden als „public“ behandelt.  Weitere Informationen finden Sie unter [Sichtbarkeitsoptionen für Gruppen](#group-visibility-options).<br>Die Sichtbarkeit kann nur beim Erstellen einer Gruppe festgelegt und anschließend nicht mehr bearbeitet werden.<br>Sichtbarkeit wird nur für einheitliche Gruppen unterstützt. Für Sicherheitsgruppen wird sie nicht unterstützt.|

### <a name="group-visibility-options"></a>Sichtbarkeitsoptionen für Gruppen

Im Folgenden wird die Bedeutung der einzelnen Werte der Eigenschaft **visibility** erläutert:
 
|Wert|Beschreibung|
|:----|-----------|
| `public` | Jeder kann der Gruppe beitreten, ohne dass die Berechtigung „Besitzer“ erforderlich ist.<br>Jeder kann die Inhalte der Gruppe anzeigen.|
| `private` | Die Berechtigung „Besitzer“ ist erforderlich, um der Gruppe beizutreten.<br>Nichtmitglieder können die Inhalte der Gruppe nicht anzeigen.|
| `hiddenmembership` | Die Berechtigung „Besitzer“ ist erforderlich, um der Gruppe beizutreten.<br>Nichtmitglieder können die Inhalte der Gruppe nicht anzeigen.<br>Nichtmitglieder können die Mitglieder der Gruppe nicht sehen.<br>Administratoren (global, Unternehmen, Benutzer und Helpdesk) können die Mitgliedschaft der Gruppe anzeigen.<br>Die Gruppe wird im globalen Adressbuch (GAL) angezeigt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md)-Sammlung|Die Liste der Benutzer oder Gruppen, die berechtigt sind, Beiträge oder Kalenderereignisse in dieser Gruppe zu erstellen. Wenn diese Liste nicht leer ist, dürfen nur die hier aufgeführten Benutzer oder Gruppen Beiträge schreiben.|
|Kalender|[Kalender](calendar.md)|Der Kalender der Gruppe. Schreibgeschützt.|
|calendarView|[Ereignissammlung](event.md)|Die Kalenderansicht für den Kalender. Schreibgeschützt.|
|conversations|[Unterhaltungssammlung](conversation.md)|Die Unterhaltungen der Gruppe|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Der Benutzer (bzw. die Anwendung), der/die Gruppe erstellt hat. HINWEIS: Dies ist nicht festgelegt, wenn der Benutzer ein Administrator ist. Schreibgeschützt.|
|Laufwerk|[drive](drive.md)|Das Standardlaufwerk der Gruppe. Schreibgeschützt.|
|drives|[drive](drive.md)-Sammlung|Die Laufwerke der Gruppe. Schreibgeschützt.|
|endpoints|[endpoint](endpoint.md)-Sammlung| Endpunkte für die Gruppe. Schreibgeschützt. Nullwerte zulassend.|
|events|[event](event.md)-Sammlung|Die Ereignisse der Gruppe.|
|extensions|[extension](extension.md)-Sammlung|Die Sammlung der für die Gruppe definierten offenen Erweiterungen. Schreibgeschützt. Nullwerte zulassend.|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung|Die Sammlung der Lebenszyklusrichtlinien für diese Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Gruppen und administrative Einheiten, in denen dieser Benutzer Mitglied ist. HTTP-Methoden: GET (für alle Gruppen unterstützt). Schreibgeschützt. Lässt NULL-Werte zu.|
|members|[directoryObject](directoryobject.md)-Sammlung| Benutzer, Kontakte und Gruppen, die Mitglieder dieser Gruppe sind. HTTP-Methoden: GET (für alle Gruppen unterstützt), POST (für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt), DELETE (nur für Sicherheitsgruppen unterstützt). Schreibgeschützt. Nullwerte zulassend.|
|membersWithLicenseErrors|[User](user.md)-Sammlung|Eine Liste von Gruppenmitgliedern mit Lizenzfehlern aus dieser gruppenbasierten Lizenzizenzzuweisung. Schreibgeschützt.|
|onenote|[OneNote](onenote.md)| Schreibgeschützt.|
|owners|[directoryObject](directoryobject.md)-Sammlung|Die Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind und die berechtigt sind, dieses Objekt zu ändern. HTTP-Methoden: GET (für alle Gruppen unterstützt), POST (für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt), DELETE (nur für Sicherheitsgruppen unterstützt). Schreibgeschützt. Nullwerte zulassend.|
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto der Gruppe. |
|Fotos|[profilePhoto](profilephoto.md)-Sammlung| Die Profilfotos im Besitz der  Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|planner|[plannerGroup](plannergroup.md)| Selektive Planner-Dienste, die für die Gruppe zur Verfügung stehen. Schreibgeschützt. Nullwerte zulassend. |
|rejectedSenders|[directoryObject](directoryobject.md)-Sammlung|Die Liste der Benutzer oder Gruppen, die nicht berechtigt sind, Beiträge oder Kalenderereignisse in dieser Gruppe zu erstellen. Lässt NULL-Werte zu|
|settings|[directorySetting](directorysetting.md) collection| Einstellungen, die das Verhalten dieser Gruppe steuern, z. B. ob Mitglieder Gastbenutzer zur Gruppe einladen können. Nullwerte zulassend.|
|sites|[site](site.md)-Sammlung|Die Liste der SharePoint-Websites in dieser Gruppe. Der Zugriff auf die Standardwebsite erfolgt mit „/sites/root“.|
|threads|[conversationThread](conversationthread.md)-Sammlung| Die Unterhaltungs-Threads der Gruppe. Lässt NULL-Werte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",    
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isFavorite": true,  
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": ["string"],
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
