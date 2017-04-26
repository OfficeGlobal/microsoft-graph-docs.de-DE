# <a name="get-incremental-changes-for-users-preview"></a>Inkrementelle Änderungen für Benutzer abrufen (Vorschau)

Mit der [Delta-Abfrage](./delta_query_overview.md) können Sie Ergänzungen, Löschungen oder Aktualisierungen an Benutzern anhand einer Serie von [Delta](../api-reference/beta/api/user_delta.md)-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Benutzern ermitteln, ohne den gesamten Satz von Benutzern von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.

Die Delta-Abfrage unterstützt die vollständige Synchronisierung, die alle Benutzer in einem Mandanten abruft, und die inkrementelle Synchronisierung, die nur die Benutzer abruft, die seit der letzten Synchronisierung geändert wurden. In der Regel führen Sie zunächst eine vollständige Synchronisierung aller Benutzer in einem Mandanten durch und rufen anschließend regelmäßig inkrementelle Änderungen an Benutzern ab. 

## <a name="tracking-user-changes"></a>Nachverfolgen von Benutzeränderungen

Das Nachverfolgen von Benutzeränderungen ist eine Runde aus einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Eine GET-Anforderung wird ähnlich wie das [Auflisten von Benutzern](../api-reference/beta/api/user_list.md) durchgeführt, außer dass Folgendes eingeschlossen wird:

- Die **Delta**-Funktion.
- Ein [Statustoken](./delta_query_overview.md) (_deltaToken_ oder _skipToken_) aus dem vorherigen GET-**Delta**-Funktionsaufruf.

## <a name="example"></a>Beispiel

Das folgende Beispiel zeigt eine Serienanforderung zum Nachverfolgen von Änderungen an Benutzern:

1. [Ursprüngliche Anforderung](#initial-request) und [Antwort](#initial-response)
2. [nextLink-Anforderung](#nextlink-request) und [Antwort](#nextlink-response)
3. [Letzte nextLink-Anforderung](#final-nextlink-request) und [Antwort](#final-nextlink-response)
4. [deltaLink-Anforderung](#deltalink-request) und [deltaLink-Antwort](#deltalink-response)

## <a name="initial-request"></a>Ursprüngliche Anforderung

Um Änderungen an der Benutzerressource nachzuverfolgen, nehmen Sie zunächst eine Anforderung einschließlich der Delta-Funktion für die Benutzerressource vor. 

Beachten Sie Folgendes:

- Der optionale Abfrageparameter „$select“ wird in die Anforderung eingeschlossen, um zu veranschaulichen, wie Abfrageparameter automatisch in zukünftige Anforderungen eingeschlossen werden.
- Die ursprüngliche Anforderung enthält kein Statustoken. Statustoken werden in nachfolgenden Anforderungen verwendet.

``` http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,givenName,surname
```

### <a name="initial-response"></a>Ursprüngliche Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das Sammlungsobjekt [user](../api-reference/beta/resources/user.md) im Antworttext zurückgegeben. Wenn der ganze Satz von Benutzern zu groß ist, enthält die Antwort zudem ein nextLink-Statustoken.

In diesem Beispiel wird eine nextLink-URL zurückgegeben, die angibt, dass es zusätzliche Seiten mit Daten gibt, die in der Sitzung abgerufen werden müssen. Der Abfrageparameter „$select“ aus der ursprünglichen Anforderung wird in der nextLink-URL codiert.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a>nextLink-Anforderung

Die zweite Anforderung gibt das aus der vorherigen Antwort zurückgegebene `skipToken` an. Beachten Sie, dass der Parameter `$select` nicht erforderlich ist, da das `skipToken` ihn codiert und einschließt.

``` http
GET https://graph.microsoft.com/beta/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a>nextLink-Antwort

Die Antwort enthält einen `nextLink` und ein weiteres `skipToken`, wodurch angegeben wird, dass weitere Benutzer verfügbar sind. Sie nehmen weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Letzte nextLink-Anforderung

Die dritte Anforderung verwendet weiterhin das neueste aus der letzten Synchronisierungsanforderung zurückgegebene `skipToken`. 

``` http
GET https://graph.microsoft.com/beta/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhaOYDE2VPA4vxIPA90-P6OzGd6Rvku5fDgBRIGS
```

## <a name="final-nextlink-response"></a>Letzte nextLink-Antwort

Wenn die deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten. Speichern Sie das `deltaToken`, und verwenden Sie es in der Anforderungs-URL, um Änderungen an Benutzern zu ermitteln. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/beta/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a>deltaLink-Anforderung

Mit dem `deltaToken` aus der [letzten Antwort](#final-nextlink-response) können Sie seit der letzten Anforderung geänderte (hinzugefügte, gelöschte oder aktualisierte) Benutzer abrufen.

``` http
GET https://graph.microsoft.com/beta/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>deltaLink-Antwort

Falls keine Änderungen vorgenommen wurden, wird dasselbe `deltatoken` ohne Ergebnisse zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/beta/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": []
}
```

Wenn Änderungen vorgenommen wurden, wird dasselbe `deltatoken` mit einer Sammlung der geänderten Benutzer zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/beta/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "removed":"changed",
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d"
    }
}
```
## <a name="see-also"></a>Siehe auch
[Microsoft Graph-Delta-Abfrage](../concepts/delta_query_overview.md) – Übersicht.