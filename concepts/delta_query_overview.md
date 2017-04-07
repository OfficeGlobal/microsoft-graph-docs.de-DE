#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data-preview"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten (Vorschau)

Mit der Delta-Abfrage können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Mit der Delta-Abfrage können Microsoft Graph-Anwendungen Änderungen effizient mit einem lokalen Datenspeicher synchronisieren.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in einer Ressourcensammlung

Das typische Abrufmuster sieht folgendermaßen aus:

1.  Die Anwendung ruft zunächst eine GET-Anforderung mit der Delta-Funktion für die gewünschte Ressource auf.
2.  Microsoft Graph sendet dann eine Antwort mit der angeforderten Ressource und einem [Statustoken](#state-tokens).

     a.  Wenn eine `nextLink`-URL zurückgegeben wird, gibt es zusätzliche Seiten mit Daten, die in der Sitzung abgerufen werden müssen. Die Anwendung nimmt weiterhin Anforderungen über die `nextLink`-URL vor, bis eine `deltaLink`-URL in der Antwort zurückgegeben wird.

     b.  Wenn eine `deltaLink`-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenden Ressource. Für zukünftige Anforderungen verwendet die Anwendung die `deltaLink`-URL, um Informationen zu Änderungen an der Ressource zu erhalten.
     
3.  Wenn die Anwendung Informationen zu Änderungen an der Ressource benötigt, nimmt sie eine neue Anforderung mit der in Schritt 2 erhaltenen `deltaLink`-URL vor. Diese Anforderung *kann* umgehend nach Abschluss von Schritt 2 oder bei der Prüfung auf Änderungen durch die Anwendung vorgenommen werden.
4.  Microsoft Graph gibt eine Antwort, in der die seit der vorherigen Anforderung an der Ressource vorgenommenen Änderungen beschrieben werden, sowie eine `nextLink`-URL oder eine `deltaLink`-URL zurück.

### <a name="state-tokens"></a>Statustoken

Eine GET-Antwort einer Delta-Abfrage umfasst immer eine URL, die in einem `nextLink`- oder `deltaLink`-Antwortheader angegeben ist. Die `nextLink`-URL umfasst ein _skipToken_, und eine `deltaLink`-URL umfasst ein _deltaToken_. 

Diese Token sind für den Client nicht transparent. Nachfolgend finden Sie alles, was Sie darüber wissen müssen:

- Jedes Token gibt den Status an und ist eine Momentaufnahme der Ressource in dieser Runde der Änderungsnachverfolgung. 
- Diese Statustoken codieren zudem weitere Abfrageparameter (wie `$select`, sofern die Ressource ihn unterstützt), die in der ursprünglichen Delta-Abfrageanforderung angegeben sind, und schließt diese ein, sodass Sie sie in nachfolgenden Delta-Abfrageanforderungen nicht wiederholen müssen.
- Beim Ausführen von Delta-Abfragen können Sie einfach die `nextLink`- oder `deltaLink`-URL unverändert kopieren und auf den nächsten **delta**-Funktionsaufruf anwenden, ohne den Inhalt der URL, einschließlich ihres Statustoken, zu überprüfen.


### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Wenn ein Client einen Abfrageparameter verwendet, muss dieser in der ursprünglichen Anforderung angegeben sein. Microsoft Graph codiert automatisch den bzw. die angegebenen Parameter in den in der Antwort enthaltenen `nextLink` oder `deltaLink`. Die aufrufende Anwendung muss die gewünschten Abfrageparameter nur einmal im Vorfeld angeben. Microsoft Graph fügt die angegebenen Parameter automatisch für alle nachfolgenden Anforderungen hinzu.

Für Benutzer und Gruppen gibt es Einschränkungen im Hinblick auf die Verwendung einiger Abfrageparameter:

-   Wenn ein `$select`-Abfrageparameter verwendet wird, bedeutet dies, dass der Kunde nur Änderungen an den Eigenschaften oder Beziehungen nachverfolgen möchte, die in der `$select`-Anweisung angegeben sind. Das heißt, wenn eine Änderung an einer nicht ausgewählten Eigenschaft vorgenommen wird, wird die Ressource, für die diese Eigenschaft geändert wurde, nach einer nachfolgenden Anforderung nicht in der Delta-Antwort angezeigt.
-   `$expand` wird nicht unterstützt.

## <a name="resource-representation-in-the-delta-query-response"></a>Ressourcendarstellung in der Delta-Abfrageantwort

-   Neu erstellte Instanzen einer unterstützten Ressourcen werden in der Delta-Abfrageantwort mithilfe ihrer standardmäßigen Darstellung dargestellt.

-   Aktualisierte Instanzen werden anhand ihrer **ID** mit *mindestens* den Eigenschaften dargestellt, die aktualisiert wurden. Es können aber auch weitere Eigenschaften eingeschlossen werden.

-   Änderungen an Beziehungen für Benutzer und Gruppen werden als Anmerkungen in der standardmäßigen Ressourcendarstellung dargestellt. Diese Anmerkungen weisen das Format `propertyName@delta` auf und werden nur angezeigt, wenn der Client explizit wählt, Änderungen an der Beziehung mithilfe des `$select`-Parameters nachzuverfolgen.

-   Entfernte Entitäten werden nur anhand ihrer **ID** und einem `@removed`-Knoten dargestellt. Der `@removed`-Knoten kann zusätzliche Informationen zum Grund der Entfernung der Entität enthalten.

> **Hinweis zu zukünftigen Änderungen**: Entfernte Instanzen werden derzeit mit dem `@removed`-Knoten im folgenden Format angezeigt: *„@removed“: „Grund für Entfernung“*. Demnächst wird jedoch eine wichtige Änderung vorgenommen. Bevor die Delta-Abfrage von /beta zu /v1.0 wechselt, wird ein Objekt in dem entfernten Knoten verschachtelt, um weitere Informationen bereitzustellen. Beispiel: *@removed {reason: „Grund für Entfernung“}*. Dieses Objekt kann zukünftig durch zusätzliche Metadaten zur Entfernung erweitert werden.

## <a name="supported-resources"></a>Unterstützte Ressourcen

Die Delta-Abfrage wird derzeit in der Vorschau für den /beta-Endpunkt von Microsoft Graph für die folgenden Ressourcen unterstützt:

| **Ressourcensammlung** | **API** |
|:------ | :------ |
| Ereignisse in einer Kalenderansicht (Datumsbereich) des primären Kalenders | [Delta](../api-reference/beta/api/event_delta.md)-Funktion der [event](../api-reference/beta/resources/event.md)-Ressource |
| Gruppen | [Delta](../api-reference/beta/api/group_delta.md)-Funktion der [group](../api-reference/beta/resources/group.md)-Ressource |
| E-Mail-Ordner | [Delta](../api-reference/beta/api/mailfolder_delta.md)-Funktion der [mailFolder](../api-reference/beta/resources/mailFolder.md)-Ressource |
| Nachrichten in einem Ordner | [Delta](../api-reference/beta/api/message_delta.md)-Funktion der [message](../api-reference/beta/resources/message.md)-Ressource | 
| Ordner mit persönlichen Kontakten | [Delta](../api-reference/beta/api/contactfolder_delta.md)-Funktion der [contactFolder](../api-reference/beta/resources/contactfolder.md)-Ressource |
| Persönliche Kontakte in einem Ordner | [Delta](../api-reference/beta/api/contact_delta.md)-Funktion der [contact](../api-reference/beta/resources/contact.md)-Ressource |
| Benutzer | [Delta](../api-reference/beta/api/user_delta.md)-Funktion der [user](../api-reference/beta/resources/user.md)-Ressource | 
| Laufwerk-Elemente\* | [Delta](../api-reference/beta/api/item_delta.md)-Funktion der [driveItem](../api-reference/beta/resources/driveItem.md)-Ressource |


> \* Das Nachverfolgen von Änderungen an Laufwerken und deren untergeordneten Elementen wird bereits in v1.0 unterstützt. Das Verwendungsmuster ähnelt den anderen unterstützten Ressourcen, mit geringen Unterschieden in der Syntax. Die Delta-Abfrage für Laufwerke wird zwecks Konsistenz mit anderen Ressourcentypen demnächst aktualisiert. Genauere Informationen zu der aktuellen Syntax finden Sie unter <https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/item_delta>

## <a name="prerequisites"></a>Voraussetzungen

Dieselben [Berechtigungen](../authorization/permission_scopes.md), die zum Lesen einer bestimmten Ressource erforderlich sind, werden auch zur Durchführung der Delta-Abfrage für diese Ressource benötigt.

## <a name="known-limitations"></a>Bekannte Einschränkungen

Das Nachverfolgen von Änderungen an Beziehungen für Benutzer und Gruppen wird nur innerhalb der spezifischen Ressourcenklasse unterstützt, für die Änderungen nachverfolgt werden. Wenn ein Client beispielsweise Änderungen an *groups* nachverfolgt und die Beziehung **members** ausgewählt ist, erhält der Client nur dann Aktualisierungen an Mitgliedschaften in der Delta-Abfrageantwort, wenn diese Mitglieder auch *groups* sind. In anderen Worten wird das Nachverfolgen der Gruppenmitgliedschaft für Benutzer noch nicht unterstützt. Das Microsoft Graph-Team weiß, dass dieses Szenario hohe Priorität hat, und eine Aktualisierung soll im März 2017 vorgenommen werden.

## <a name="delta-query-request-examples"></a>Beispiele für die Delta-Abfrageanforderung 

- [Inkrementelle Änderungen an Ereignissen in einer Kalenderansicht (Vorschau) abrufen](../Concepts/delta_query_events.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen (Vorschau)](./delta_query_messages.md)
- [Inkrementelle Änderungen an Gruppen abrufen (Vorschau)](./delta_query_groups.md)
- [Inkrementelle Änderungen an Benutzern abrufen (Vorschau)](./delta_query_users.md)