---
title: Gruppen-Ressourcentyp
description: Stellt eine Gruppe Azure Active Directory (AD Azure), die eine Office 365-Gruppe, ein Team in Microsoft-Teams, eine dynamische Gruppe oder eine Sicherheitsgruppe sein kann.
ms.openlocfilehash: a1a200918c34f5e2fa220a88d3c69871d6b93ad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064490"
---
# <a name="group-resource-type"></a>Gruppen-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Gruppe Azure Active Directory (AD Azure), die eine Office 365-Gruppe, ein Team in Microsoft-Teams, eine dynamische Gruppe oder eine Sicherheitsgruppe sein kann.
Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).
- Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user-delta.md)-Funktion.

> **Microsoft-Teams und Office 365 Gruppen unterstützen die Zusammenarbeit von Gruppen**. Sie können die meisten der Office 365-API-Gruppen mit Microsoft-Teams verwenden. Um ein [Team](team.md), erste [Gruppe erstellen](../api/group-post-groups.md) und dann auf [Hinzufügen ein Team, um es](../api/team-put-teams.md)zu erstellen. Weitere Informationen hierzu finden Sie unter [Übersicht über die Microsoft-Teams](teams-api-overview.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|**Gruppenverwaltung**| | |
|[Gruppe erstellen](../api/group-post-groups.md) | [Gruppe](group.md) |Erstellen einer neuen Gruppe wie angegeben. Sie können eine Gruppe von Office 365, dynamische Gruppe, Sicherheitsgruppe oder Team sein.|
|[Gruppe abrufen](../api/group-get.md) | [Gruppe](group.md) |Eigenschaften lesen und Beziehungen des Group-Objekt.|
|[Gruppe aktualisieren](../api/group-update.md) | Keine |Aktualisiert die Eigenschaften eines Gruppenobjekts. |
|[Gruppe löschen](../api/group-delete.md) | Keiner |Löscht das Gruppenobjekt. |
|[delta](../api/group-delta.md)|group-Sammlung| Dient zum Abrufen inkrementeller Änderungen für Gruppen. |
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung| Dient zum Auflisten der Gruppenlebenszyklusrichtlinien. |
|[Besitzer auflisten](../api/group-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Eigentümer der Gruppe aus der **owners**-Navigationseigenschaft ab.|
|[Add owner](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| Fügt einen neuen Besitzer zur Gruppe durch Bereitstellen an die **owners**-Navigationseigenschaft bereit (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Besitzer entfernen](../api/group-delete-owners.md) | Keiner |Entfernt einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe über die **owners**-Navigationseigenschaft.|
|[Mitglieder auflisten](../api/group-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer und Gruppen, die direkte Mitglieder dieser Gruppe sind, aus der **members**-Navigationseigenschaft ab.|
|[Transitive Listenmitglieder](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie die Benutzer, Gruppen, Geräte und Service-Prinzipale, die Mitglieder, einschließlich geschachtelter Mitglieder dieser Gruppe sind.|
|[Mitglied hinzufügen](../api/group-post-members.md) |[directoryObject](directoryobject.md)| Fügt dieser Gruppe einen Benutzer oder eine Gruppe durch Bereitstellung an die **members**-Navigationseigenschaft hinzu (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Mitglied entfernen](../api/group-delete-members.md) | Keine |Entfernt ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe anhand der **members**-Navigationseigenschaft. Sie können Benutzer oder andere Gruppen entfernen. |
|[memberOf auflisten](../api/group-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie die Gruppen und administrative Einheiten, die dieser Gruppe ein direktes Mitglied in der Navigationseigenschaft Mitglied ist.|
|[Transitive Mitglied Liste](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Liste der Gruppen und administrative Einheiten, denen dieser Benutzer ein Mitglied ist. Dieser Vorgang ist transitiv und enthält die Gruppen, denen dieser Gruppe geschachtelte Mitglied ist. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Zeichenfolgenauflistung|Überprüfen Sie die Mitgliedschaft in einer Liste von Gruppen. Die Funktion ist transitiv.|
|[getMemberGroups](../api/group-getmembergroups.md)|Zeichenfolgenauflistung|Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist. Die Funktion ist transitiv.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Zeichenfolgenauflistung|Zurückgeben Sie aller Gruppen und administrative Einheiten, denen die Gruppe ein Mitglied ist. Die Funktion ist transitiv. |
|[Einstellung erstellen](../api/directorysetting-post-settings.md) | [Verzeichnisberechtigungen](directorysetting.md) |Erstellen einer Einstellungsobjekt basierend auf einer DirectorySettingTemplate. Die POST-Anforderung muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben. Für diesen Vorgang dürfen nur bestimmten Gruppen-Vorlagen verwendet werden.|
|[Einstellung abrufen](../api/directorysetting-get.md) | [Verzeichnisberechtigungen](directorysetting.md) |Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.|
|[Einstellungen auflisten](../api/directorysetting-list.md) | [Verzeichnisberechtigungen](directorysetting.md) -Auflistung |Listet Eigenschaften aller Einstellungsobjekte auf.|
|[Einstellung aktualisieren](../api/directorysetting-update.md) | [Verzeichnisberechtigungen](directorysetting.md)  |Aktualisiert ein Einstellungsobjekt. |
|[Einstellung löschen](../api/directorysetting-delete.md) | Keine |Löscht ein Einstellungsobjekt. |
|[Endpunkte auflisten](../api/group-list-endpoints.md) |[Endpunkt](endpoint.md) -Auflistung| Rufen Sie eine Auflistung der Endpunkt-Objekts. |
|[Get-Endpunkt](../api/endpoint-get.md) | [Endpunkt](endpoint.md) | Lesen Sie Eigenschaften und Beziehungen eines Endpunkts-Objekts. |
|[delta](../api/group-delta.md)|group-Sammlung| Dient zum Abrufen inkrementeller Änderungen für Gruppen. |
|[validateProperties](../api/group-validateproperties.md)|JSON| Anzeigenamen ein Office 365-Gruppe zu überprüfen, oder e-Mail-Spitzname naming Richtlinien entspricht. | 
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
|[Thread löschen](../api/group-delete-thread.md) |Keine| Löschen Sie die Thread-Objekt
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
|[Liste joinedTeams](../api/user-list-joinedteams.md) |[Gruppensammlung](group.md)| Rufen Sie die Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.|
|[subscribeByMail](../api/group-subscribebymail.md)|Keine|Die IsSubscribedByMail-Eigenschaft auf **true**festgelegt. Aktivieren den aktuellen Benutzer zum Empfangen von e-Mail-Unterhaltungen. Unterstützt nur die Office 365-Gruppen.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Keine|Legen Sie die IsSubscribedByMail-Eigenschaft auf **false fest**. Deaktivieren den aktuellen Benutzer aus e-Mail-Unterhaltungen empfangen. Unterstützt nur die Office 365-Gruppen.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Keine|Setzen Sie die UnseenCount auf 0 der alle Beiträge, die der aktuelle Benutzer seit seinem letzten Besuch nicht erkannt wurde. Unterstützt nur die Office 365-Gruppen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolescher Wert|Der Standardwert ist **false**. Gibt an, ob Personen außerhalb der Organisation Nachrichten an die Gruppe senden können.|
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|Die Lizenzen, die der Gruppe zugewiesen sind. Schreibgeschützt.|
|autoSubscribeNewMembers|Boolean|Der Standardwert ist **false**. Gibt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten. Sie können diese Eigenschaft in einer PATCH-Anforderung für die Gruppe festlegen; legen Sie sie nicht in der anfänglichen POST-Anforderung fest, mit der die Gruppe erstellt wird.|
|Klassifikation|String|Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrige, mittlere oder hohe geschäftliche Auswirkungen). Gültige Werte für diese Eigenschaft werden durch die Erstellung eines ClassificationList-[setting](directorysetting.md)-Werts basierend auf der [Vorlagendefinition](directorysettingtemplate.md) erstellt.|
|createdDateTime|DateTimeOffset| Zeitstempel der Gruppenerstellung. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Gruppe erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
|description|String|Eine optionale Beschreibung für die Gruppe.|
|displayName|String|Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.|
|groupTypes|Zeichenfolgenauflistung| Gibt den Typ der Gruppe zu erstellen. Mögliche Werte sind `Unified` zum Erstellen einer Gruppe Office 365 oder `DynamicMembership` für dynamische Gruppen.  Für alle anderen Gruppe Typen, wie Sicherheit-aktivierten Gruppen und e-Mail-aktivierte Sicherheitsgruppen diese Eigenschaft nicht festlegen.|
|id|String|Eindeutiger Bezeichner für die Gruppe. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|isSubscribedByMail|Boolean|Der Standardwert ist **true**. Gibt an, ob der aktuelle Benutzer den Erhalt von E-Mail-Unterhaltungen abonniert hat.|
|licenseProcessingState|String|Status der Gruppe Lizenz Zuordnung an alle Mitglieder der Gruppe angibt. Schreibgeschützt. Mögliche Werte: `QueuedForProcessing`, `ProcessingInProgress`, und `ProcessingComplete`.|
|Mail|String|Die SMTP-Adresse für die Gruppe ein, z. B. „serviceadmins@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailEnabled|Boolean|Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe.|
|mailNickname|String|Der E-Mail-Alias für die Gruppe (eindeutig in der Organisation). Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. Unterstützt $filter.|
|membershipRule|String|Die Regel, die Mitglieder dieser Gruppe bestimmt, ob die Gruppe eine dynamische Gruppe ist (GroupTypes enthält `DynamicMembership`). Weitere Informationen zur Syntax der Mitgliedschaftsregel finden Sie unter [Regeln für die Mitgliedschaft syntax](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|String|Gibt an, ob die Verarbeitung der dynamischen Mitgliedschaft ist fehlerhaft oder angehalten. Mögliche Werte sind "Auf" oder "Angehalten"|
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt das letzte Mal an dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. Unterstützt $filter.|
|onPremisesProvisioningErrors|[OnPremisesProvisioningError](onpremisesprovisioningerror.md) -Auflistung| Fehler beim Microsoft Synchronisierung während der Bereitstellung verwenden. |
|onPremisesSecurityIdentifier|String|Enthält die lokale Sicherheits-ID (SID) für die Gruppe, die von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt. |
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt. Unterstützt $filter.|
|preferredDataLocation|String|Die bevorzugte Datenspeicherort für die Gruppe. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Die bevorzugte Sprache für ein Office 365-Gruppe. Führen Sie die ISO 639-1-Code sollte; beispielsweise "En-US".|
|proxyAddresses|Zeichenfolgenauflistung| Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any** -Operator ist für Filterausdrücke auf mehrwertige Eigenschaften erforderlich. Schreibgeschützt. Lässt keine Nullwerte zu. Unterstützt $filter. |
|renewedDateTime|DateTimeOffset| Zeitstempel der letzten Verlängerung der Gruppe. Dies kann nicht direkt geändert werden und wird nur über die [Aktion zum Verlängern des Diensts](../api/grouplifecyclepolicy-renewgroup.md) aktualisiert. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|securityEnabled|Boolean|Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. Unterstützt $filter.|
|Design|String|Gibt eine Office 365-Gruppe Farbdesign an. Mögliche Werte sind `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` oder `Red`.|
|unseenConversationsCount|Int32|Anzahl der Unterhaltungen, die seit dem letzten Besuch des angemeldeten Benutzers, der Gruppe einen oder mehrere neue Beiträge bereitgestellt wurden. Diese Eigenschaft entspricht dem **UnseenCount**.|
|unseenCount|Int32|Anzahl der Unterhaltungen, die seit dem letzten Besuch des angemeldeten Benutzers, der Gruppe einen oder mehrere neue Beiträge bereitgestellt wurden. Diese Eigenschaft entspricht dem **UnseenConversationsCount**.|
|unseenMessagesCount|Int32|Anzahl der neuen Beiträge, die seit dem letzten Besuch des angemeldeten Benutzers, der Gruppe der Gruppe Unterhaltungen bereitgestellt wurden.|
|visibility|String| Gibt die Sichtbarkeit einer Office 365-Gruppe. Mögliche Werte sind: `private`, `public`, oder `hiddenmembership`; leere Werte werden als öffentliche behandelt.  Finden Sie unter [Sichtbarkeitsoptionen Gruppe](#group-visibility-options) , um mehr zu erfahren.<br>Sichtbarkeit kann festgelegt werden, nur, wenn eine Gruppe erstellt wird. Es kann nicht bearbeitet werden.<br>Sichtbarkeit wird nur für unified Gruppen unterstützt. Es ist nicht für Sicherheitsgruppen unterstützt.|

### <a name="group-visibility-options"></a>Gruppe Sichtbarkeitsoptionen

Hier ist, was bedeutet, dass jeder Wert der **Visibility** -Eigenschaft:
 
|Wert|Beschreibung|
|:----|-----------|
| `public` | Jeder kann die Gruppe ohne Besitzerberechtigung teilnehmen.<br>Jeder Benutzer kann den Inhalt der Gruppe anzeigen.|
| `private` | Besitzerberechtigung ist erforderlich, um der Gruppe "Leistungsprotokollbenutzer".<br>Nicht-Mitglieder können nicht den Inhalt der Gruppe anzeigen.|
| `hiddenmembership` | Besitzerberechtigung ist erforderlich, um der Gruppe "Leistungsprotokollbenutzer".<br>Nicht-Mitglieder können nicht den Inhalt der Gruppe anzeigen.<br>Nicht-Elemente nicht die Mitglieder der Gruppe angezeigt.<br>Administratoren (global, Unternehmen, Benutzer und Helpdesk) können die Mitgliedschaft der Gruppe anzeigen.<br>Die Gruppe wird in der globalen Adressliste (GAL).|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md)-Sammlung|Die Liste der Benutzer oder Gruppen, die berechtigt sind, Beiträge oder Kalenderereignisse in dieser Gruppe zu erstellen. Wenn diese Liste nicht leer ist, dürfen nur die hier aufgeführten Benutzer oder Gruppen Beiträge schreiben.|
|Kalender|[Kalender](calendar.md)|Der Kalender der Gruppe. Schreibgeschützt.|
|calendarView|[Ereignissammlung](event.md)|Die Kalenderansicht für den Kalender. Schreibgeschützt.|
|conversations|[Unterhaltungssammlung](conversation.md)|Die Unterhaltungen der Gruppe|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Schreibgeschützt.|
|Laufwerk|[Laufwerk](drive.md)|Das Laufwerk der Gruppe. Schreibgeschützt.|
|Endpunkte|[Endpunkt](endpoint.md) -Auflistung| Endpunkte für die Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|events|[Ereignissammlung](event.md)|Ereignisse, die der Gruppe.|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Auflistung der open-Erweiterungen für die Gruppe definiert. Lässt Nullwerte zu.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Gruppen und administrative Einheiten, denen dieser Gruppe ein Mitglied ist. HTTP-Methoden: Abrufen (unterstützt für alle Gruppen). Schreibgeschützt. Lässt Nullwerte zu.|
|Elemente|[directoryObject](directoryobject.md)-Sammlung| Benutzer, Kontakte und Gruppen, die Mitglieder dieser Gruppe sind. HTTP-Methoden: Abrufen (unterstützt für alle Gruppen), POST (unterstützt für Sicherheitsgruppen und e-Mail-aktivierten Sicherheitsgruppen), DELETE (unterstützt nur für Sicherheitsgruppen) schreibgeschützt. Lässt Nullwerte zu.|
|membersWithLicenseErrors|[Benutzer](user.md) -Auflistung|Eine Liste der Mitglieder der Gruppe mit Fehlern aus dieser Gruppe basierenden lizenzzuweisung Lizenz. Schreibgeschützt.|
|onenote|[OneNote](onenote.md)| Schreibgeschützt.|
|owners|[directoryObject](directoryobject.md)-Sammlung|Der Besitzer der Gruppe. Die Besitzer sind eine Reihe von nicht-Administrator-Benutzer, die berechtigt sind, dieses Objekt zu ändern. HTTP-Methoden: Abrufen (unterstützt für alle Gruppen), POST (unterstützt für Sicherheitsgruppen und e-Mail-aktivierten Sicherheitsgruppen), DELETE (unterstützt nur für Sicherheitsgruppen) schreibgeschützt. Lässt Nullwerte zu.|
|Foto|[profilePhoto](profilephoto.md)| Die Gruppe Profilfoto. |
|Fotos|[profilePhoto](profilephoto.md)-Sammlung| Die Profilfotos im Besitz der  Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|Planner|[plannerGroup](plannergroup.md)| Selektive Planner-Dienste für die Gruppe verfügbar. Schreibgeschützt. Lässt Nullwerte zu. |
|rejectedSenders|[directoryObject](directoryobject.md)-Sammlung|Die Liste der Benutzer oder Gruppen, die nicht berechtigt sind, Beiträge oder Kalenderereignisse in dieser Gruppe zu erstellen. Lässt NULL-Werte zu|
|Einstellungen|[Verzeichnisberechtigungen](directorysetting.md) -Auflistung| Die Einstellungen, die dieser Gruppe Verhalten, z. B., ob Mitglieder von Gastbenutzern zur Gruppe einladen können steuern können. Lässt Nullwerte zu.|
|sites|[site](site.md)-Sammlung|Die Liste der SharePoint-Websites in dieser Gruppe. Der Zugriff auf die Standardwebsite erfolgt mit „/sites/root“.|
|threads|[conversationThread](conversationthread.md)-Sammlung| Die Unterhaltungs-Threads der Gruppe. Lässt NULL-Werte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Der folgende Code ist ein JSON-Darstellung der Ressource

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
