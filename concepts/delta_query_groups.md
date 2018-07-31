# <a name="get-incremental-changes-for-groups"></a>Dient zum Abrufen inkrementeller Änderungen für Gruppen.

Mit der [Delta-Abfrage](./delta_query_overview.md) können Sie Ergänzungen, Löschungen oder Aktualisierungen an Gruppen anhand von einer Serie von [Delta](../api-reference/v1.0/api/group_delta.md)-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Gruppen ermitteln, ohne den gesamten Satz von Gruppen von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.

Clients, die Gruppen mit einem lokalen Profilspeicher synchronisieren, können Delta Abfragen für die anfängliche vollständige Synchronisierung und für inkrementelle Synchronisierungen in der Zukunft verwenden. In der Regel führt ein Client eine anfängliche vollständige Synchronisierung aller Gruppen in einem Mandanten durch und ruft anschließend regelmäßig inkrementelle Änderungen an Gruppen ab.

## <a name="tracking-group-changes"></a>Nachverfolgen von Gruppenänderungen

Das Nachverfolgen von Gruppenänderungen ist eine Runde von einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Eine GET-Anforderung wird ähnlich wie das [Auflisten von Gruppen](../api-reference/v1.0/api/group_list.md) durchgeführt, außer dass Folgendes eingeschlossen wird:

- Die **Delta**-Funktion.
- Ein [Statustoken](./delta_query_overview.md) (*deltaToken* oder *skipToken*) aus dem vorherigen GET-**Delta**-Funktionsaufruf.

## <a name="example"></a>Beispiel

Das folgende Beispiel zeigt eine Serienanforderung zum Nachverfolgen von Änderungen an Gruppen:

1. [Ursprüngliche Anforderung](#initial-request) und [Antwort](#initial-response)
2. [nextLink-Anforderung](#nextlink-request) und [Antwort](#nextlink-response)
3. [Letzte nextLink-Anforderung](#final-nextlink-request) und [Antwort](#final-nextlink-response)
4. [deltaLink-Anforderung](#deltalink-request) und [deltaLink-Antwort](#deltalink-response)

## <a name="initial-request"></a>Ursprüngliche Anforderung

Um Änderungen an der Gruppenressource nachzuverfolgen, nehmen Sie zunächst eine Anforderung einschließlich der Delta-Funktion für die Gruppenressource vor.

Beachten Sie Folgendes:

- Der optionale `$select`-Abfrageparameter wird in die Anforderung eingeschlossen, um zu veranschaulichen, wie Abfrageparameter automatisch in zukünftige Anforderungen eingeschlossen werden.
- Der optionale `$expand`-Abfrageparameter wird eingeschlossen, um anzuzeigen, wie Mitglieder der Gruppe zusammen mit Objekten der Gruppe abgerufen werden können. Dadurch können Änderungen der Mitgliedschaft nachverfolgt werden, wenn z. B. Benutzer zu Gruppen hinzugefügt oder daraus entfernt werden.
- Die ursprüngliche Anforderung enthält kein Statustoken. Statustoken werden in nachfolgenden Anforderungen verwendet.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

## <a name="initial-response"></a>Ursprüngliche Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../api-reference/v1.0/resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben. Wenn der gesamte Gruppensatz zu groß ist, um in eine Antwort zu passen, wird ebenfalls ein `nextLink` mit einem Statustoken eingeschlossen.

In diesem Beispiel wurde ein `nextLink` eingeschlossen; die ursprünglichen `$select`- und `$expand`-Abfrageparameter werden im Statustoken codiert.

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
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**Hinweis:** Die `members@delta`-Eigenschaft ist im ersten Gruppenobjekts – TestGroup1 – enthalten und enthält die beiden aktuellen Mitglieder der Gruppe. TestGroup2 enthält diese Eigenschaft nicht, da die Gruppe keine Mitglieder besitzt.

## <a name="nextlink-request"></a>nextLink-Anforderung

Die zweite Anforderung verwendet `nextLink` aus der vorherigen Antwort, die `skipToken` enthält. Beachten Sie, dass die `$select`- und `$expand` -Parameter nicht explizit vorhanden sind, da sie im Token codiert werden.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>nextLink-Antwort

Die Antwort enthält ein weiteres `nextLink` mit einem neuen `skipToken`-Wert, wodurch angegeben wird, dass weitere Gruppen verfügbar sind. Sie nehmen weiterhin Anforderungen über die `nextLink`-URL vor, bis eine `deltaLink`-URL in der endgültigen Antwort zurückgegeben wird.

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
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Letzte nextLink-Anforderung

Die dritte Anforderung verwendet erneut die neueste `nextLink`.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Letzte nextLink-Antwort

Zum Schluss wird die `deltaLink`-URL zurückgegeben, was bedeutet, dass keine weitere Daten für den vorhandenen Status von Gruppen vorhanden sind. Für künftige Anforderungen verwendet die Anwendung die enthaltenen Werte `deltaLink` und `deltaToken`, um neue Änderungen an Gruppen abzufragen.

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

Mit dem `deltaLink` aus der [letzten Antwort](#final-nextlink-response) können Sie seit der letzten Anforderung vorgenommene Änderungen an Gruppen abrufen. Dazu gehören:
- Neu erstelle Gruppenobjekte
- Gelöschte Gruppenobjekte
- Gruppenobjekte, für die eine Eigenschaft geändert wurde (z. B. **displayName** wurde geändert).
- Gruppenobjekte, für die Mitgliedsobjekte hinzugefügt oder entfernt wurden.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>deltaLink-Antwort

Falls keine Änderungen vorgenommen wurden, wird `deltaLink` ohne Ergebnisse zurückgegeben – die Eigenschaft `value` ist leer. Stellen Sie sicher, dass Sie den vorherigen Link in der Anwendung durch den neuen für die Verwendung in kommenden Anrufen ersetzen.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Wenn Änderungen vorgenommen wurden, ist eine Sammlung der geänderten Gruppen enthalten. Die Antwort enthält zudem `nextLink` – falls mehrere Seiten mit Änderungen abgerufen werden müssen – oder `deltaLink`. Sie sollten nach `nextLinks` das gleiche Muster implementieren wie zuvor und die endgültige Eigenschaft `deltaLink` für zukünftige Anrufe beibehalten.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```
Einige Punkte, die Sie bei der oben aufgeführten Beispielantwort beachten sollten:
- Die Objekte werden mit demselben Eigenschaftensatz zurückgegeben, der ursprünglich mit den Abfrageparametern `$select` und `$expand` angegeben wurde.
- Es sind sowohl geänderte als auch nicht geänderte Eigenschaften enthalten. Im Beispiel oben hat die Eigenschaft `description` einen neuen Wert, während die Eigenschaft `displayName` nicht geändert wurde.
- `members@delta` enthält alle Änderungen an der Mitgliedschaft.
  - Der erste Benutzer in der Liste wurde aus der Gruppe entfernt – entweder durch Entfernen der Mitgliedschaft oder durch Löschen des Benutzerobjekts selbst. Die Eigenschaft `@removed` beschreibt dies.
  - Der zweite Benutzer wurde zur Gruppe hinzugefügt.

## <a name="paging-through-members-in-a-large-group"></a>Blättern durch Mitglieder in einer großen Gruppe
Die Eigenschaft `members@delta` ist standardmäßig in Gruppenobjekten enthalten, wenn der Abfrageparameter `$select` nicht angegeben oder der Parameter `$expand=members` explizit angegeben wird. Bei Gruppen mit vielen Mitgliedern ist es möglich, dass nicht alle Mitglieder in eine einzelne Antwort passen. In diesem Abschnitt beschreiben wir das Muster, das Sie in solchen Fällen implementieren sollten.

>**Hinweis:** Dieses Muster bezieht sich sowohl auf den anfänglichen Abruf des Gruppenzustands als auch auf nachfolgende Aufrufe zum Abrufen von Delta-Änderungen.

Nehmen wir an, dass Sie die folgende Delta-Abfrage ausführen, um entweder den kompletten Anfangszustand der Gruppe oder zu einem späteren Zeitpunkt die Delta-Änderungen abzufragen:

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

1. Microsoft Graph gibt möglicherweise eine Antwort zurück, die nur ein Gruppenobjekt mit einer langen Liste von Mitgliedern in der Eigenschaft `members@delta` enthält:

**Erste Seite**

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. Wenn Sie `nextLink` folgen, erhalten Sie möglicherweise erneut eine Antwort mit demselben Gruppenobjekt. Die gleichen Eigenschaftswerte werden zurückgegeben, aber die erweiterte Eigenschaft `members@delta` enthält jetzt eine andere Benutzerliste.

**Zweite Seite**

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. Schließlich wird auf diese Weise die gesamten Mitgliederliste zurückgegeben, und andere Gruppen werden in der Antwort angezeigt.

Es wird empfohlen, die folgenden bewährten Methoden zu verwenden, um dieses Muster zu verarbeiten:
- Folgen Sie stets `nextLink` und führen Sie den Zustand jeder Gruppe lokal zusammen: Wenn Sie Antworten im Zusammenhang mit der gleichen Gruppe erhalten haben, verwenden Sie diese, um in Ihrer Anwendung die komplette Mitgliederliste zu erstellen.
- Es empfiehlt sich, bei den Antworten von keiner bestimmten Sequenz auszugehen. Gehen Sie davon aus, dass die gleiche Gruppe an einer beliebigen Stelle in der Sequenz `nextLink` angezeigt werden kann und berücksichtigen Sie dies in Ihrer Zusammenführungslogik.


## <a name="see-also"></a>Siehe auch
[Microsoft Graph-Delta-Abfrage](../concepts/delta_query_overview.md) – Übersicht.
