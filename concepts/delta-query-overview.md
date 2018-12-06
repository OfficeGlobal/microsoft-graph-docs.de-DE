---
title: Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten
description: Mit der Delta-Abfrage können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Mit der Delta-Abfrage können Microsoft Graph-Anwendungen Änderungen effizient mit einem lokalen Datenspeicher synchronisieren.
ms.openlocfilehash: 4732cabed3595738b70c54a7a029f19400edbe6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092327"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten

Mit der Delta-Abfrage können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Mit der Delta-Abfrage können Microsoft Graph-Anwendungen Änderungen effizient mit einem lokalen Datenspeicher synchronisieren.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in einer Ressourcensammlung

Das typische Abrufmuster sieht folgendermaßen aus:

1. Die Anwendung ruft zunächst eine GET-Anforderung mit der Delta-Funktion für die gewünschte Ressource auf.
2. Microsoft Graph sendet dann eine Antwort mit der angeforderten Ressource und einem [Statustoken](#state-tokens).

     a.  Wenn eine `nextLink`-URL zurückgegeben wird, müssen eventuell zusätzliche Seiten mit Daten in der Sitzung abgerufen werden. Die Anwendung nimmt weiterhin Anforderungen über die `nextLink`-URL vor, um alle Seiten mit Daten abzurufen, bis eine `deltaLink`-URL in der Antwort zurückgegeben wird.

     b.  Wenn eine `deltaLink`-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenden Ressource. Für zukünftige Anforderungen verwendet die Anwendung die `deltaLink`-URL, um Informationen zu Änderungen an der Ressource zu erhalten.

3. Wenn die Anwendung Informationen zu Änderungen an der Ressource benötigt, nimmt sie eine neue Anforderung mit der in Schritt 2 erhaltenen `deltaLink`-URL vor. Diese Anforderung *kann* umgehend nach Abschluss von Schritt 2 oder bei der Prüfung auf Änderungen durch die Anwendung vorgenommen werden.
4. Microsoft Graph gibt eine Antwort, in der die seit der vorherigen Anforderung an der Ressource vorgenommenen Änderungen beschrieben werden, sowie eine `nextLink`-URL oder eine `deltaLink`-URL zurück.

>**Hinweis:** In Azure Active Directory gespeicherte Ressourcen (z. B. Benutzer und Gruppen) unterstützen Szenarien im Zusammenhang mit „Synchronisieren ab jetzt“. Deshalb können Sie die Schritte 1 und 2 oben überspringen (wenn Sie nicht den vollständigen Status der Ressource abrufen möchten) und stattdessen den neuesten `deltaLink` abrufen. Fügen Sie `$deltaToken=latest` an die `delta`-Funktion an; die Antwort enthält dann ein `deltaLink` und keine Ressourcendaten.

### <a name="state-tokens"></a>Statustoken

Eine GET-Antwort einer Delta-Abfrage umfasst immer eine URL, die in einem `nextLink`- oder `deltaLink`-Antwortheader angegeben ist. Die `nextLink`-URL umfasst ein _skipToken_, und eine `deltaLink`-URL umfasst ein _deltaToken_.

Diese Token sind für den Client nicht transparent. Nachfolgend finden Sie alles, was Sie darüber wissen müssen:

- Jedes Token gibt den Status an und ist eine Momentaufnahme der Ressource in dieser Runde der Änderungsnachverfolgung.

- Die Statustoken codieren und umfassen auch andere Abfrageparameter (z. B. `$select`), die in der anfänglichen Delta-Abfrageanforderung angegeben sind. Es ist daher nicht erforderlich, diese in nachfolgenden Delta-Abfrageanforderungen zu wiederholen.

- Beim Ausführen von Delta-Abfragen können Sie die `nextLink`- oder `deltaLink`-URL kopieren und auf den nächsten **delta**-Funktionsaufruf anwenden, ohne den Inhalt der URL, einschließlich ihres Statustoken, zu überprüfen.

### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Wenn ein Client einen Abfrageparameter verwendet, muss dieser in der ursprünglichen Anforderung angegeben sein. Microsoft Graph codiert automatisch den angegebenen Parameter in den in der Antwort enthaltenen `nextLink` oder `deltaLink`. Die aufrufende Anwendung muss die gewünschten Abfrageparameter nur einmal im Vorfeld angeben. Microsoft Graph fügt die angegebenen Parameter automatisch für alle nachfolgenden Anforderungen hinzu.

Für Benutzer und Gruppen gibt es Einschränkungen im Hinblick auf die Verwendung einiger Abfrageparameter:

- Wenn ein `$select`-Abfrageparameter verwendet wird, bedeutet dies, dass der Client nur Änderungen an den Eigenschaften oder Beziehungen nachverfolgen möchte, die in der `$select`-Anweisung angegeben sind. Wenn eine Änderung an einer nicht ausgewählten Eigenschaft vorgenommen wird, wird die Ressource, für die diese Eigenschaft geändert wurde, nach einer nachfolgenden Anforderung nicht in der Delta-Antwort angezeigt.
- `$expand` wird nur für die Navigationseigenschaften `manager` und `members` jeweils für Benutzer und Gruppen unterstützt.

- Mit Bereichsfiltern können Sie Änderungen an einem oder mehreren bestimmten Benutzern bzw. einer oder mehreren bestimmten Gruppen nach objectId nachverfolgen. Die folgende Anforderung gibt beispielsweise Änderungen für die Gruppen zurück, die mit den im Abfragefilter angegebenen IDs übereinstimmen: https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'

## <a name="resource-representation-in-the-delta-query-response"></a>Ressourcendarstellung in der Delta-Abfrageantwort

- Neu erstellte Instanzen einer unterstützten Ressourcen werden in der Delta-Abfrageantwort mithilfe ihrer standardmäßigen Darstellung dargestellt.

- Aktualisierte Instanzen werden anhand ihrer **ID** mit *mindestens* den Eigenschaften dargestellt, die aktualisiert wurden. Es können aber auch weitere Eigenschaften eingeschlossen werden.

- Beziehungen für Benutzer und Gruppen werden als Anmerkungen in der standardmäßigen Ressourcendarstellung dargestellt. Diese Anmerkungen haben das Format `propertyName@delta`. Die Anmerkungen sind in der Antwort auf die erste Delta-Abfrageanforderung enthalten.

Entfernte Instanzen werden durch ihre **ID** und ein `@removed`-Objekt dargestellt. Das `@removed`-Objekt kann zusätzliche Informationen zum Grund der Entfernung der Instanz enthalten. Beispiel: "@removed": {"reason": "changed"}.

Mögliche @removed-Gründe sind *changed* und *deleted*.

- *Changed* gibt an, dass das Element gelöscht wurde und aus [deletedItems](/graph/api/resources/directory?view=graph-rest-beta) wiederhergestellt werden kann.

- *Deleted* gibt an, dass das Element gelöscht wurde und nicht wiederhergestellt werden kann.

Das `@removed`-Objekt kann in der Antwort auf die erste Delta-Abfrage und in nachverfolgten (deltaLink-)Antworten zurückgegeben werden. Clients, die Delta-Abfrageanforderungen verwenden, sollten so konzipiert sein, dass sie diese Objekte in den Antworten behandeln.

## <a name="supported-resources"></a>Unterstützte Ressourcen

Die Delta-Abfrage wird derzeit für die folgenden Ressourcen unterstützt:

| **Ressourcensammlung** | **API** |
|:------ | :------ |
| Anwendungen (Vorschau) | [Delta](/graph/api/application-delta?view=graph-rest-beta)-Funktion der [application](/graph/api/resources/application?view=graph-rest-beta)-Ressource (Vorschau) |
| Verzeichnisobjekte | [Delta](/graph/api/directoryobject-delta?view=graph-rest-beta)-Funktion der [directoryObjects](/graph/api/resources/directoryobject?view=graph-rest-beta)-Ressource (Vorschau) |
| Verzeichnisrollen | [Delta](/graph/api/directoryrole-delta?view=graph-rest-1.0)-Funktion der [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0)-Ressource (Vorschau) |
| Ereignisse in einer Kalenderansicht (Datumsbereich) des primären Kalenders | [Delta](/graph/api/event-delta?view=graph-rest-1.0)-Funktion der [event](/graph/api/resources/event?view=graph-rest-1.0)-Ressource |
| Gruppen | [Delta](/graph/api/group-delta?view=graph-rest-1.0)-Funktion der [group](/graph/api/resources/group?view=graph-rest-1.0)-Ressource |
| E-Mail-Ordner | [Delta](/graph/api/mailfolder-delta?view=graph-rest-1.0)-Funktion der [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)-Ressource |
| Nachrichten in einem Ordner | [Delta](/graph/api/message-delta?view=graph-rest-1.0)-Funktion der [message](/graph/api/resources/message?view=graph-rest-1.0)-Ressource |
| Ordner mit persönlichen Kontakten | [Delta](/graph/api/contactfolder-delta?view=graph-rest-1.0)-Funktion der [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)-Ressource |
| Persönliche Kontakte in einem Ordner | [Delta](/graph/api/contact-delta?view=graph-rest-1.0)-Funktion der [contact](/graph/api/resources/contact?view=graph-rest-1.0)-Ressource |
| Dienstprinzipale (Vorschau) | [Delta](/graph/api/serviceprincipal-delta?view=graph-rest-beta)-Funktion der [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta)-Ressource (Vorschau) |
| Benutzer | [Delta](/graph/api/user-delta?view=graph-rest-1.0)-Funktion der [user](/graph/api/resources/user?view=graph-rest-1.0)-Ressource |
| Laufwerk-Elemente\* | [Delta](/graph/api/driveitem-delta?view=graph-rest-1.0)-Funktion der [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)-Ressource |
| Planner-Elemente\*\* | [Delta](/graph/api/planneruser-list-delta?view=graph-rest-beta)-Funktion des all-Segments der [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta)-Ressource (Vorschau) |

> \* Das Verwendungsmuster für OneDrive-Ressourcen ähnelt dem der anderen unterstützten Ressourcen, mit geringen Unterschieden in der Syntax. Die Delta-Abfrage für Laufwerke wird zwecks Konsistenz mit anderen Ressourcentypen demnächst aktualisiert. Weitere Informationen zur aktuellen Syntax finden Sie unter[Laufwerksänderungen nachverfolgen](/graph/api/item-delta?view=graph-rest-1.0).

> \*\* Das Verwendungsmuster für Planner-Ressourcen ähnelt anderen unterstützten Ressourcen bis auf ein paar Unterschiede.  Weitere Informationen finden Sie unter [Änderungen für Planner nachverfolgen](/graph/api/planneruser-list-delta?view=graph-rest-beta).

## <a name="prerequisites"></a>Voraussetzungen

Dieselben [Berechtigungen](./permissions-reference.md), die zum Lesen einer bestimmten Ressource erforderlich sind, werden auch zur Durchführung der Delta-Abfrage für diese Ressource benötigt.

## <a name="delta-query-request-examples"></a>Beispiele für die Delta-Abfrageanforderung

- [Inkrementelle Änderungen an Ereignissen in einer Kalenderansicht abrufen](delta-query-events.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](./delta-query-messages.md)
- [Inkrementelle Änderungen an Gruppen abrufen](./delta-query-groups.md)
- [Inkrementelle Änderungen an Benutzern abrufen](./delta-query-users.md)
