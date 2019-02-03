---
title: Gruppen-Ressourcentyp
description: Stellt eine Azure Active Directory (Azure AD)-Gruppe dar, bei der es sich um eine Office 365-Gruppe, eine dynamische Gruppe oder eine Sicherheitsgruppe handeln kann.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aa3dd6974a0e75661b91d155a19bd197d3fe742e
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2019
ms.locfileid: "29690952"
---
# <a name="group-resource-type"></a>Gruppen-Ressourcentyp

Stellt eine Azure Active Directory-Gruppe (Azure AD) dar, bei der es sich um eine Office 365-Gruppe, eine dynamische Gruppe oder eine Sicherheitsgruppe handeln kann. Erbt von [directoryObject](directoryobject.md).

Aus Leistungsgründen geben die Vorgänge [create](../api/group-post-groups.md), [get](../api/group-get.md) und [list](../api/group-list.md) standardmäßig nur eine Teilmenge häufig verwendeter Eigenschaften zurück. Diese _Standard_eigenschaften werden im Abschnitt [Eigenschaften](#properties) aufgeführt. Zum Abrufen von Eigenschaften, die nicht standardmäßig zurückgegeben werden, geben sie diese in einer OData-Abfrageoption `$select` an. Sehen Sie sich das [Beispiel](../api/group-get.md#request-2) an.

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften als [Erweiterungen](/graph/extensibility-overview).
- Abonnieren von [Änderungsbenachrichtigungen](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user-delta.md)-Funktion.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|**Gruppenverwaltung**| | |
|[Gruppe erstellen](../api/group-post-groups.md) | [Gruppe](group.md) |Erstellt eine neue Gruppe. Dabei kann es sich um eine Office 365-Gruppe, eine dynamische Gruppe oder eine Sicherheitsgruppe handeln.|
|[Gruppe abrufen](../api/group-get.md) | [Gruppe](group.md) |Liest die Eigenschaften eines Gruppenobjekts.|
|[Gruppen auflisten](../api/group-list.md) |[Gruppensammlung](group.md) |Listet Gruppenobjekte und deren Eigenschaften auf.|
|[Gruppe aktualisieren](../api/group-update.md) | Keine |Aktualisiert die Eigenschaften eines Gruppenobjekts. |
|[Gruppe löschen](../api/group-delete.md) | Keiner |Löscht das Gruppenobjekt. |
|[delta](../api/group-delta.md)|group-Sammlung| Dient zum Abrufen inkrementeller Änderungen für Gruppen. |
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung| Dient zum Auflisten der Gruppenlebenszyklusrichtlinien. |
|[Renew](../api/group-renew.md)|Boolescher Wert|Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.|
|[Add owner](../api/group-post-owners.md) |Keine| Fügt einen neuen Besitzer zur Gruppe durch Bereitstellen an die **owners**-Navigationseigenschaft bereit (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Besitzer auflisten](../api/group-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Eigentümer der Gruppe aus der **owners**-Navigationseigenschaft ab.|
|[Besitzer entfernen](../api/group-delete-owners.md) | Keiner |Entfernt einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe über die **owners**-Navigationseigenschaft.|
|[Mitglied hinzufügen](../api/group-post-members.md) |Keiner| Fügt dieser Gruppe einen Benutzer oder eine Gruppe durch Bereitstellung an die **members**-Navigationseigenschaft hinzu (wird nur für Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen unterstützt).|
|[Mitglieder auflisten](../api/group-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer und Gruppen, die direkte Mitglieder dieser Gruppe sind, aus der **members**-Navigationseigenschaft ab.|
|[Transitive Mitglieder auflisten](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer, Gruppen und Geräte ab, die Mitglieder sind, einschließlich der geschachtelten Mitglieder dieser Gruppe.|
|[Transitive memberOf auflisten](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Listet die Gruppen auf, deren Mitglied der Benutzer ist. Dieser Vorgang ist transitiv und schließt die Gruppen ein, in denen diese Gruppe ein geschachteltes Mitglied. |
|[Mitglied entfernen](../api/group-delete-members.md) | Keine |Entfernt ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-fähigen Sicherheitsgruppe anhand der **members**-Navigationseigenschaft. Sie können Benutzer oder andere Gruppen entfernen. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection|Prüft die Mitgliedschaft dieser Gruppe in einer Liste von Gruppen. Die Funktion ist transitiv.|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist. Die Funktion ist transitiv.|
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection|Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist. Die Funktion ist transitiv. |
|[Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Erstellen Sie eine Einstellungsobjekt basierend auf einer groupSettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Für diesen Vorgang können nur gruppenspezifische Vorlagen verwendet werden.|
|[Einstellung abrufen](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts. |
|[Einstellungen auflisten](../api/groupsetting-list.md) | [groupSetting](groupsetting.md)-Sammlung | Listet Eigenschaften aller Einstellungsobjekte auf. |
|[Einstellung aktualisieren](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Aktualisiert ein Einstellungsobjekt. |
|[Einstellung löschen](../api/groupsetting-delete.md) | Keine | Löscht ein Einstellungsobjekt. |
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
|[Thread löschen](../api/group-delete-thread.md) |Keine| Löscht das Threadobjekt.|
|[acceptedSenders auflisten](../api/group-list-acceptedsenders.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der acceptedSenders für diese Gruppe befinden.|
|[acceptedSender hinzufügen](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Fügt einen Benutzer oder eine Gruppe zur acceptSenders-Sammlung hinzu.|
|[acceptedSender entfernen](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Entfernt einen Benutzer oder eine Gruppe aus der acceptedSenders-Sammlung.|
|[rejectedSenders auflisten](../api/group-list-rejectedsenders.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft eine Liste von Benutzern oder Gruppen ab, die sich in der Liste der rejectedSenders für diese Gruppe befinden.|
|[rejectedSender hinzufügen](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Sammlung hinzu.|
|[rejectedSender entfernen](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Entfernt einen neuen Benutzer oder eine neue Gruppe aus der rejectedSenders-Sammlung.|
|[Einstellung erstellen](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Erstellen Sie eine Einstellungsobjekt basierend auf einer groupSettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Für diesen Vorgang können nur gruppenspezifische Vorlagen verwendet werden.|
|[Einstellung abrufen](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts. |
|[Einstellungen auflisten](../api/groupsetting-list.md) | [groupSetting](groupsetting.md)-Sammlung | Listet Eigenschaften aller Einstellungsobjekte auf. |
|[Einstellung aktualisieren](../api/groupsetting-update.md) | Keine | Aktualisiert ein Einstellungsobjekt. |
|[Einstellung löschen](../api/groupsetting-delete.md) | Keine | Löscht ein Einstellungsobjekt. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Andere Gruppenressourcen**| | |
|[Fotos auflisten](../api/group-list-photos.md) |[profilePhoto](photo.md)-Sammlung| Ruft eine Sammlung von Profilfotos für die Gruppe ab.|
|[plannerPlans auflisten](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md)-Sammlung| Ruft Plannerer-Pläne im Besitz der Gruppe ab.|
|**Benutzereinstellungen**| | |
|[addFavorite](../api/group-addfavorite.md)|Keine|Fügt die Gruppe zu der Liste der Favoritengruppen des angemeldeten Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.|
|[removeFavorite](../api/group-removefavorite.md)|Keine|Entfernt die Gruppe aus der Liste der Favoritengruppen des angemeldeten Benutzers. Wird nur für Office 365-Gruppen unterstützt.|
|[memberOf auflisten](../api/group-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Gruppen und administrativen Einheiten, bei denen dieser Benutzer direktes Mitglied ist, aus der **memberOf**-Navigationseigenschaft ab.|
|[subscribeByMail](../api/group-subscribebymail.md)|Keiner|Legt die isSubscribedByMail-Eigenschaft auf **true** fest. Aktiviert den angemeldeten Benutzer für den Erhalt von E-Mail-Unterhaltungen. Wird nur für Office 365-Gruppen unterstützt.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Keiner|Legt die isSubscribedByMail-Eigenschaft auf **false** fest. Deaktiviert den angemeldeten Benutzer für den Erhalt von E-Mail-Unterhaltungen. Wird nur für Office 365-Gruppen unterstützt.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Keine|Setzt das unseenCount-Element aller Beiträge, die der angemeldete Benutzer seit dem letzten Besuch noch nicht gesehen hat, auf 0 zurück. Wird nur für Office 365-Gruppen unterstützt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolesch| Gibt an, ob Personen außerhalb der Organisation Nachrichten an die Gruppe senden können. Der Standardwert lautet **false**. <br><br>Wird nur für $select zurückgegeben. |
|assignedLicenses|[assignedLicense](assignedlicense.md)-Sammlung|Die Lizenzen, die der Gruppe zugewiesen sind. <br><br>Wird nur für $select zurückgegeben. Schreibgeschützt.|
|autoSubscribeNewMembers|Boolesch|Gibt an, ob neu zur Gruppe hinzugefügte Mitglieder automatisch E-Mail-Benachrichtigungen erhalten. Sie können diese Eigenschaft in einer PATCH-Anforderung für die Gruppe festlegen; legen Sie sie nicht in der anfänglichen POST-Anforderung fest, mit der die Gruppe erstellt wird. Der Standardwert lautet **false**. <br><br>Wird nur für $select zurückgegeben.|
|classification|Zeichenfolge|Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrige, mittlere oder hohe geschäftliche Auswirkungen). Gültige Werte für diese Eigenschaft werden durch die Erstellung eines ClassificationList-[setting](groupsetting.md)-Werts basierend auf der [Vorlagendefinition](groupsettingtemplate.md) erstellt.<br><br>Wird standardmäßig zurückgegeben.|
|createdDateTime|DateTimeOffset| Zeitstempel der Gruppenerstellung. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Gruppe erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. |
|description|String|Eine optionale Beschreibung für die Gruppe. <br><br>Wird standardmäßig zurückgegeben.|
|displayName|Zeichenfolge|Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht gelöscht werden. <br><br>Wird standardmäßig zurückgegeben. Unterstützt $filter und $orderby. |
|groupTypes|Zeichenfolgenauflistung| Gibt den Typ der zu erstellenden Gruppe an. Mögliche Werte sind `Unified` zum Erstellen einer Office 365-Gruppe oder `DynamicMembership` für dynamische Gruppen.  Legen Sie für alle anderen Gruppentypen wie Gruppen mit aktivierter Sicherheit und E-Mail-fähige Sicherheitsgruppen diese Eigenschaft nicht fest. <br><br>Wird standardmäßig zurückgegeben. Unterstützt $filter.|
|hasMembersWithLicenseErrors|Boolesch|Gibt an, ob es in dieser Gruppe Mitglieder mit Lizenzfehlern aus ihrer gruppenbasierten Lizenzzuweisung gibt. <br><br>Diese Eigenschaft wird nie bei einem GET-Vorgang zurückgegeben. Sie können sie als $filter-Argument verwenden, um Gruppen abzurufen, die Mitglieder mit Lizenzfehlern enthalten (d. h., Sie filtern nach dieser Eigenschaft mit dem Wert true). Sehen Sie sich das [Beispiel](../api/group-list.md) an.|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Gruppe. <br><br>Wird standardmäßig zurückgegeben. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|isSubscribedByMail|Boolesch|Gibt an, ob der angemeldete Benutzer den Erhalt von E-Mail-Unterhaltungen abonniert hat. Der Standardwert ist **true**. <br><br>Wird nur für $select zurückgegeben. |
|licenseProcessingState|Zeichenfolge|Gibt den Status der Gruppenlizenzzuweisung an alle Mitglieder der Gruppe an. Der Standardwert lautet **false**. Schreibgeschützt. Mögliche Werte: `QueuedForProcessing`, `ProcessingInProgress` und `ProcessingComplete`.<br><br>Wird nur für $select zurückgegeben. Schreibgeschützt.|
|mail|Zeichenfolge|Die SMTP-Adresse für die Gruppe, z. B. „serviceadmins@contoso.onmicrosoft.com“. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. Unterstützt $filter.|
|mailEnabled|Boolesch|Gibt an, ob es sich bei der Gruppe um eine E-Mail-fähige Gruppe handelt. Wenn die **securityEnabled**-Eigenschaft auch auf **true** festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls handelt es sich bei der Gruppe um eine Microsoft Exchange-Verteilergruppe. <br><br>Wird standardmäßig zurückgegeben.|
|mailNickname|Zeichenfolge|Der E-Mail-Alias für die Gruppe, in der Organisation eindeutig. Diese Eigenschaft muss beim Erstellen einer Gruppe angegeben werden. <br><br>Wird standardmäßig zurückgegeben. Unterstützt $filter.|
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis an. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. Unterstützt $filter.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)-Sammlung| Fehler bei Verwendung eines Microsoft-Synchronisierungsprodukts während der Bereitstellung. <br><br>Wird standardmäßig zurückgegeben.|
|onPremisesSecurityIdentifier|Zeichenfolge|Enthält die lokale Sicherheits-ID (SID) für die Gruppe, die von der lokalen Bereitstellung in der Cloud synchronisiert wurde. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. |
|onPremisesSyncEnabled|Boolean|**true**, wenn diese Gruppe aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn die Gruppe ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. Unterstützt $filter.|
|preferredDataLocation|Zeichenfolge|Der bevorzugte Datenspeicherort für die Gruppe. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Wird standardmäßig zurückgegeben.|
|proxyAddresses|Zeichenfolgenauflistung| E-Mail-Adressen für die Gruppe, die in das gleiche Gruppenpostfach umgeleitet werden sollen. Zum Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt. Lässt keine NULL-Werte zu. Unterstützt $filter. |
|renewedDateTime|DateTimeOffset| Zeitstempel der letzten Verlängerung der Gruppe. Dies kann nicht direkt geändert werden und wird nur über die [Aktion zum Verlängern des Diensts](../api/group-renew.md) aktualisiert. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. <br><br>Wird standardmäßig zurückgegeben. Schreibgeschützt.|
|securityEnabled|Boolean|Gibt an, ob es sich bei der Gruppe um eine Sicherheitsgruppe handelt. Wenn die **mailEnabled**-Eigenschaft auch auf „true“ festgelegt ist, handelt es sich bei der Gruppe um eine E-Mail-fähige Sicherheitsgruppe; andernfalls ist die Gruppe eine Sicherheitsgruppe. Muss für Office 365-Gruppen auf **false** festgelegt sein. <br><br>Wird standardmäßig zurückgegeben. Unterstützt $filter.|
|unseenCount|Int32|Die Anzahl von Unterhaltungen, die neue Beiträge erhalten haben, da der angemeldete Benutzer die Gruppe zuletzt besucht hat. <br><br>Wird nur für $select zurückgegeben. |
|visibility|Zeichenfolge| Gibt die Sichtbarkeit einer Office 365-Gruppe an. Mögliche Werte sind: `private`, `public` oder `hiddenmembership`; leere Werte werden als „public“ behandelt.  Weitere Informationen finden Sie unter [Sichtbarkeitsoptionen für Gruppen](#group-visibility-options).<br>Die Sichtbarkeit kann nur beim Erstellen einer Gruppe festgelegt und anschließend nicht mehr bearbeitet werden.<br>Sichtbarkeit wird nur für einheitliche Gruppen unterstützt. Für Sicherheitsgruppen wird sie nicht unterstützt. <br><br>Wird standardmäßig zurückgegeben.|


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
|events|[Ereignissammlung](event.md)|Die Kalenderereignisse der Gruppe.|
|extensions|[extension](extension.md)-Sammlung|Die Sammlung der für die Gruppe definierten offenen Erweiterungen. Schreibgeschützt. Nullwerte zulassend.|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung|Die Sammlung der Lebenszyklusrichtlinien für diese Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Gruppen, bei denen diese Gruppe Mitglied ist. HTTP-Methoden: GET (unterstützt für alle Gruppen). Schreibgeschützt. Lässt NULL-Werte zu.|
|Elemente|[directoryObject](directoryobject.md)-Sammlung| Benutzer und Gruppen, die Mitglieder dieser Gruppe sind. HTTP-Methoden: GET (unterstützt für alle Gruppen), POST (unterstützt für Office 365-Gruppen, Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen), DELETE (unterstützt für Office 365-Gruppen und Sicherheitsgruppen), lässt NULL-Werte zu.|
|membersWithLicenseErrors|[User](user.md)-Sammlung|Eine Liste von Gruppenmitgliedern mit Lizenzfehlern aus dieser gruppenbasierten Lizenzizenzzuweisung. Schreibgeschützt.|
|onenote|[Onenote](onenote.md)| Schreibgeschützt.|
|owners|[directoryObject](directoryobject.md)-Sammlung|Die Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind und die berechtigt sind, dieses Objekt zu ändern. Beschränkt auf 10 Besitzer. HTTP-Methoden: GET (unterstützt für alle Gruppen), POST (unterstützt für Office 365-Gruppen, Sicherheitsgruppen und E-Mail-fähige Sicherheitsgruppen), DELETE (unterstützt für Office 365-Gruppen und Sicherheitsgruppen). Lässt NULL-Werte zu.|
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto der Gruppe. |
|Fotos|[profilePhoto](profilephoto.md)-Sammlung| Die Profilfotos im Besitz der  Gruppe. Schreibgeschützt. Lässt Nullwerte zu.|
|planner|[plannerGroup](plannergroup.md)| Einstiegspunkt der Planner-Ressource, die möglicherweise für eine einheitliche Gruppe vorhanden ist.|
|rejectedSenders|[directoryObject](directoryobject.md)-Sammlung|Die Liste der Benutzer oder Gruppen, die nicht berechtigt sind, Beiträge oder Kalenderereignisse in dieser Gruppe zu erstellen. Lässt NULL-Werte zu|
|Einstellungen|[groupSetting](groupsetting.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|sites|[site](site.md)-Sammlung|Die Liste der SharePoint-Websites in dieser Gruppe. Der Zugriff auf die Standardwebsite erfolgt mit „/sites/root“.|
|threads|[conversationThread](conversationthread.md)-Sammlung| Die Unterhaltungs-Threads der Gruppe. Lässt NULL-Werte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "hasMembersWithLicenseErrors": "Boolean",
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenCount": 1024,
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
