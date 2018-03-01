#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten

Mit der Delta-Abfrage können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Mit der Delta-Abfrage können Microsoft Graph-Anwendungen Änderungen effizient mit einem lokalen Datenspeicher synchronisieren.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in einer Ressourcensammlung

Das typische Abrufmuster sieht folgendermaßen aus:

1.  Die Anwendung ruft zunächst eine GET-Anforderung mit der Delta-Funktion für die gewünschte Ressource auf.
2.  Microsoft Graph sendet dann eine Antwort mit der angeforderten Ressource und einem [Statustoken](#state-tokens).

     a.  Wenn eine `nextLink`-URL zurückgegeben wird, müssen eventuell zusätzliche Seiten mit Daten in der Sitzung abgerufen werden. Die Anwendung nimmt weiterhin Anforderungen über die `nextLink`-URL vor, um alle Seiten mit Daten abzurufen, bis eine `deltaLink`-URL in der Antwort zurückgegeben wird.

     b.  Wenn eine `deltaLink`-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenden Ressource. Für zukünftige Anforderungen verwendet die Anwendung die `deltaLink`-URL, um Informationen zu Änderungen an der Ressource zu erhalten.
     
3.  Wenn die Anwendung Informationen zu Änderungen an der Ressource benötigt, nimmt sie eine neue Anforderung mit der in Schritt 2 erhaltenen `deltaLink`-URL vor. Diese Anforderung *kann* umgehend nach Abschluss von Schritt 2 oder bei der Prüfung auf Änderungen durch die Anwendung vorgenommen werden.
4.  Microsoft Graph gibt eine Antwort, in der die seit der vorherigen Anforderung an der Ressource vorgenommenen Änderungen beschrieben werden, sowie eine `nextLink`-URL oder eine `deltaLink`-URL zurück.

### <a name="state-tokens"></a>Statustoken

Eine GET-Antwort einer Delta-Abfrage umfasst immer eine URL, die in einem `nextLink`- oder `deltaLink`-Antwortheader angegeben ist. Die `nextLink`-URL umfasst ein _skipToken_, und eine `deltaLink`-URL umfasst ein _deltaToken_. 

Diese Token sind für den Client nicht transparent. Nachfolgend finden Sie alles, was Sie darüber wissen müssen:

- Jedes Token gibt den Status an und ist eine Momentaufnahme der Ressource in dieser Runde der Änderungsnachverfolgung. 
- Die Statustoken codieren und umfassen auch andere Abfrageparameter (z. B. `$select`), die in der anfänglichen Delta-Abfrageanforderung angegeben sind. Es ist daher nicht erforderlich, diese in nachfolgenden Delta-Abfrageanforderungen zu wiederholen.
- Beim Ausführen von Delta-Abfragen können Sie die `nextLink`- oder `deltaLink`-URL kopieren und auf den nächsten **delta**-Funktionsaufruf anwenden, ohne den Inhalt der URL, einschließlich ihres Statustoken, zu überprüfen.


### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Wenn ein Client einen Abfrageparameter verwendet, muss dieser in der ursprünglichen Anforderung angegeben sein. Microsoft Graph codiert automatisch den angegebenen Parameter in den in der Antwort enthaltenen `nextLink` oder `deltaLink`. Die aufrufende Anwendung muss die gewünschten Abfrageparameter nur einmal im Vorfeld angeben. Microsoft Graph fügt die angegebenen Parameter automatisch für alle nachfolgenden Anforderungen hinzu.

Für Benutzer und Gruppen gibt es Einschränkungen im Hinblick auf die Verwendung einiger Abfrageparameter:

-   Wenn ein `$select`-Abfrageparameter verwendet wird, bedeutet dies, dass der Client nur Änderungen an den Eigenschaften oder Beziehungen nachverfolgen möchte, die in der `$select`-Anweisung angegeben sind. Wenn eine Änderung an einer nicht ausgewählten Eigenschaft vorgenommen wird, wird die Ressource, für die diese Eigenschaft geändert wurde, nach einer nachfolgenden Anforderung nicht in der Delta-Antwort angezeigt.
-   `$expand` wird nicht unterstützt.

APIs für Benutzer und Gruppen können Sie mithilfe von Bereichsfiltern Änderungen an einem oder mehreren bestimmten Benutzern bzw. einer oder mehreren bestimmten Gruppen nach objectId nachverfolgen. Die folgende Anforderung gibt beispielsweise Änderungen für die Gruppen zurück, die mit den im Abfragefilter angegebenen IDs übereinstimmen: https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' oder id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e 

## <a name="resource-representation-in-the-delta-query-response"></a>Ressourcendarstellung in der Delta-Abfrageantwort

-   Neu erstellte Instanzen einer unterstützten Ressourcen werden in der Delta-Abfrageantwort mithilfe ihrer standardmäßigen Darstellung dargestellt.

-   Aktualisierte Instanzen werden anhand ihrer **ID** mit *mindestens* den Eigenschaften dargestellt, die aktualisiert wurden. Es können aber auch weitere Eigenschaften eingeschlossen werden.

-   Beziehungen für Benutzer und Gruppen werden als Anmerkungen in der standardmäßigen Ressourcendarstellung dargestellt. Diese Anmerkungen haben das Format `propertyName@delta`. Die Anmerkungen sind in der Antwort auf die erste Delta-Abfrageanforderung enthalten.

Entfernte Instanzen werden durch ihre **ID** und ein `@removed`-Objekt dargestellt. Das `@removed`-Objekt kann zusätzliche Informationen zum Grund der Entfernung der Instanz enthalten. Beispiel: "@removed": {"reason": "changed"}.

Mögliche @removed-Gründe sind *changed* und *deleted*.
- *Changed* gibt an, dass das Element gelöscht wurde und aus [deletedItems](../api-reference/beta/resources/directory.md) wiederhergestellt werden kann.
- *Deleted* gibt an, dass das Element gelöscht wurde und nicht wiederhergestellt werden kann.

Das `@removed`-Objekt kann in der Antwort auf die erste Delta-Abfrage und in nachverfolgten (deltaLink-)Antworten zurückgegeben werden. Clients, die Delta-Abfrageanforderungen verwenden, sollten so konzipiert sein, dass sie diese Objekte in den Antworten behandeln.

## <a name="supported-resources"></a>Unterstützte Ressourcen

Die Delta-Abfrage wird derzeit für die folgenden Ressourcen unterstützt:

| **Ressourcensammlung** | **API** |
|:------ | :------ |
| Ereignisse in einer Kalenderansicht (Datumsbereich) des primären Kalenders | [Delta](../api-reference/v1.0/api/event_delta.md)-Funktion der [event](../api-reference/v1.0/resources/event.md)-Ressource |
| Gruppen | [Delta](../api-reference/v1.0/api/group_delta.md)-Funktion der [group](../api-reference/v1.0/resources/group.md)-Ressource |
| E-Mail-Ordner | [Delta](../api-reference/v1.0/api/mailfolder_delta.md)-Funktion der [mailFolder](../api-reference/v1.0/resources/mailFolder.md)-Ressource |
| Nachrichten in einem Ordner | [Delta](../api-reference/v1.0/api/message_delta.md)-Funktion der [message](../api-reference/v1.0/resources/message.md)-Ressource | 
| Ordner mit persönlichen Kontakten | [Delta](../api-reference/v1.0/api/contactfolder_delta.md)-Funktion der [contactFolder](../api-reference/v1.0/resources/contactfolder.md)-Ressource |
| Persönliche Kontakte in einem Ordner | [Delta](../api-reference/v1.0/api/contact_delta.md)-Funktion der [contact](../api-reference/v1.0/resources/contact.md)-Ressource |
| Benutzer | [Delta](../api-reference/v1.0/api/user_delta.md)-Funktion der [user](../api-reference/v1.0/resources/user.md)-Ressource | 
| Laufwerk-Elemente\* | [Delta](../api-reference/v1.0/api/driveitem_delta.md)-Funktion der [driveItem](../api-reference/v1.0/resources/driveitem.md)-Ressource |


> \* Das Verwendungsmuster für OneDrive-Ressourcen ähnelt dem der anderen unterstützten Ressourcen, mit geringen Unterschieden in der Syntax. Die Delta-Abfrage für Laufwerke wird zwecks Konsistenz mit anderen Ressourcentypen demnächst aktualisiert. Weitere Informationen zur aktuellen Syntax finden Sie unter[Laufwerksänderungen nachverfolgen](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/api/item_delta).

## <a name="prerequisites"></a>Voraussetzungen

Dieselben [Berechtigungen](./permissions_reference.md), die zum Lesen einer bestimmten Ressource erforderlich sind, werden auch zur Durchführung der Delta-Abfrage für diese Ressource benötigt.

## <a name="delta-query-request-examples"></a>Beispiele für die Delta-Abfrageanforderung 

- [Inkrementelle Änderungen an Ereignissen in einer Kalenderansicht abrufen](../concepts/delta_query_events.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](./delta_query_messages.md)
- [Inkrementelle Änderungen an Gruppen abrufen](./delta_query_groups.md)
- [Inkrementelle Änderungen an Benutzern abrufen](./delta_query_users.md)
