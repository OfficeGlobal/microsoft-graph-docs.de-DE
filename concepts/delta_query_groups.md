# <a name="get-incremental-changes-for-groups"></a>Dient zum Abrufen inkrementeller Änderungen für Gruppen.

Mit der [Delta-Abfrage](./delta_query_overview.md) können Sie Ergänzungen, Löschungen oder Aktualisierungen an Gruppen anhand von einer Serie von [Delta](../api-reference/v1.0/api/group_delta.md)-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Gruppen ermitteln, ohne den gesamten Satz von Gruppen von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.

Clients, die Gruppen mit einem lokalen Profilspeicher synchronisieren, können Delta Abfragen für die anfängliche vollständige Synchronisierung und für inkrementelle Synchronisierungen in der Zukunft verwenden. In der Regel führt ein Client eine anfängliche vollständige Synchronisierung aller Gruppen in einem Mandanten durch und ruft anschließend regelmäßig inkrementelle Änderungen an Gruppen ab. 

## <a name="tracking-group-changes"></a>Nachverfolgen von Gruppenänderungen

Das Nachverfolgen von Gruppenänderungen ist eine Runde von einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Eine GET-Anforderung wird ähnlich wie das [Auflisten von Gruppen](../api-reference/v1.0/api/group_list.md) durchgeführt, außer dass Folgendes eingeschlossen wird:

- Die **Delta**-Funktion.
- Ein [Statustoken](./delta_query_overview.md) (_deltaToken_ oder _skipToken_) aus dem vorherigen GET-**Delta**-Funktionsaufruf.

## <a name="example"></a>Beispiel

Das folgende Beispiel zeigt eine Serienanforderung zum Nachverfolgen von Änderungen an Gruppen:

1. [Ursprüngliche Anforderung](#initial-request) und [Antwort](#initial-response)
2. [nextLink-Anforderung](#nextlink-request) und [Antwort](#nextlink-response)
3. [Letzte nextLink-Anforderung](#final-nextlink-request) und [Antwort](#final-nextlink-response)
4. [deltaLink-Anforderung](#deltalink-request) und [deltaLink-Antwort](#deltalink-response)

## <a name="initial-request"></a>Ursprüngliche Anforderung

Um Änderungen an der Gruppenressource nachzuverfolgen, nehmen Sie zunächst eine Anforderung einschließlich der Delta-Funktion für die Gruppenressource vor. 

Beachten Sie Folgendes:

- Der optionale Abfrageparameter „$select“ wird in die Anforderung eingeschlossen, um zu veranschaulichen, wie Abfrageparameter automatisch in zukünftige Anforderungen eingeschlossen werden.
- Die ursprüngliche Anforderung enthält kein Statustoken. Statustoken werden in nachfolgenden Anforderungen verwendet.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description
```

## <a name="initial-response"></a>Ursprüngliche Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das Sammlungsobjekt [group](../api-reference/v1.0/resources/group.md) im Antworttext zurückgegeben. Wenn der ganze Satz von Gruppen zu groß ist, enthält die Antwort zudem ein nextLink-Statustoken.

In diesem Beispiel wird eine nextLink-URL zurückgegeben, was bedeutet, dass es zusätzliche Seiten mit Daten gibt, die in der Sitzung abgerufen werden müssen. Der Abfrageparameter „$select“ aus der ursprünglichen Anforderung wird in der nextLink-URL codiert.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink-Anforderung

Die zweite Anforderung gibt das aus der vorherigen Antwort zurückgegebene `skipToken` an. Beachten Sie, dass der Parameter `$select` nicht erforderlich ist, da das `skipToken` ihn codiert und einschließt.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink-Antwort

Die Antwort enthält einen `nextLink` und ein weiteres `skipToken`, wodurch angegeben wird, dass weitere Gruppen verfügbar sind. Sie nehmen weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Letzte nextLink-Anforderung

Die dritte Anforderung verwendet weiterhin das neueste aus der letzten Synchronisierungsanforderung zurückgegebene `skipToken`. 

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Letzte nextLink-Antwort

Wenn die deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten. Speichern Sie das `deltaToken`, und verwenden Sie es in der Anforderungs-URL, um Änderungen an Gruppen zu ermitteln. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink-Anforderung

Mit dem `deltaToken` aus der [letzten Antwort](#final-nextlink-response) können Sie seit der letzten Anforderung geänderte (hinzugefügte, gelöschte oder aktualisierte) Gruppen abrufen.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink-Antwort

Falls keine Änderungen vorgenommen wurden, wird dasselbe `deltatoken` ohne Ergebnisse zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Wenn Änderungen vorgenommen wurden, wird dasselbe `deltatoken` mit einer Sammlung der geänderten Gruppen zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a>Siehe auch
[Microsoft Graph-Delta-Abfrage](../concepts/delta_query_overview.md) – Übersicht.