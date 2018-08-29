# <a name="get-incremental-changes-to-messages-in-a-folder"></a>Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen

Mit der Delta-Abfrage können Sie Ergänzungen, Löschungen oder Aktualisierungen an Nachrichten in einem Ordner anhand einer Serie von [Delta](../api-reference/v1.0/api/message_delta.md)-Funktionsaufrufen abfragen. Mit Delta-Daten können Sie einen lokalen Speicher für Nachrichten eines Benutzers pflegen und synchronisieren, ohne dass Sie jedes Mal den gesamten Nachrichtensatz vom Server abrufen müssen.

Die Delta-Abfrage unterstützt die vollständige Synchronisierung, die alle Nachrichten in einem Ordner abruft (z. B. im Posteingang des Benutzers), und die inkrementelle Synchronisierung, die alle Nachrichten abruft, die seit der letzten Synchronisierung in diesem Ordner geändert wurden. In der Regel führen Sie erst eine vollständige Synchronisierung aller Nachrichten in einem Ordner durch und rufen anschließend regelmäßig inkrementelle Änderungen an dem Ordner ab.

## <a name="track-message-changes-in-a-folder"></a>Nachverfolgen von Nachrichtenänderungen in einem Ordner

Die Delta-Abfrage wird jeweils für einen Ordner durchgeführt. Um die Änderungen der Nachrichten in einer Ordnerhierarchie nachzuverfolgen, müssen Sie jeden Ordner einzeln nachverfolgen.

Das Nachverfolgen von Nachrichtenänderungen in einem Ordner ist in der Regel eine Runde aus einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Die ursprüngliche GET-Anforderung wird ähnlich wie das [Abrufen von Nachrichten](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages) durchgeführt, außer dass die folgende **delta**-Funktion eingeschlossen wird:

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

Eine GET-Anforderung mit der **delta**-Funktion gibt Folgendes zurück:

- `nextLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _skipToken_) oder
- `deltaLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _deltaToken_).

Diese Token sind [Statustoken](delta_query_overview.md#state-tokens), die für den Client nicht transparent sind. Um mit einer Änderungsnachverfolgung fortzufahren, kopieren Sie die von der letzten GET-Anforderung zurückgegebene URL einfach und wenden sie auf den nächsten **delta**-Funktionsaufruf für denselben Ordner an.  `deltaLink` (in einer Antwort zurückgegeben), bedeutet, dass die aktuelle Runde der Änderungsnachverfolgung abgeschlossen ist. Sie können die `deltaLink`-URL für die nächste Runde speichern und verwenden.

Im [Beispiel](#example-to-synchronize-messages-in-a-folder) unten finden Sie Informationen zur Verwendung der `nextLink`- und `deltaLink`-URLs.

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>Verwenden von Abfrageparametern in einer Delta-Abfrage für Nachrichten

- Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft `id` wird immer zurückgegeben.
- Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Nachrichten.
- Es besteht eingeschränkte Unterstützung für `$filter` und `$orderby`:
  - Es werden nur die `$filter`-Ausdrücke `$filter=receivedDateTime+ge+{value}` oder `$filter=receivedDateTime+gt+{value}` unterstützt.
  - Es wird nur der `$orderby`-Ausdruck `$orderby=receivedDateTime+desc` unterstützt. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet.
- `$search` wird nicht unterstützt.

### <a name="optional-request-header"></a>Optionaler Anforderungsheader

Jede GET-Anforderung der Delta-Abfrage gibt eine Sammlung aus einer oder mehreren Nachrichten in der Antwort zurück. Sie können optional den Anforderungsheader, `Prefer: odata.maxpagesize={x}`, angeben, um die maximale Anzahl an Nachrichten in einer Antwort festzulegen.

<!--
### Iterative process

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative
process (steps 2-6) described below will return the entire set of messages in that folder.

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header,
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned
   in _@odata.nextLink_, which includes a _skipToken_.

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages,
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3.

6. When you eventually receive a _deltaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This
round of change tracking is complete.

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated)
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a>Beispiel für die Synchronisierung von Nachrichten in einem Ordner

Das folgende Beispiel zeigt zwei Synchronisierungsvorgänge für einen bestimmten Ordner, der anfänglich fünf Nachrichten enthält.

Der erste Vorgang umfasst eine Reihe von drei Anforderungen zur Synchronisierung aller fünf Nachrichten im Ordner:

- [Beispiel für ursprüngliche Anforderung](#sample-initial-request) und [Antwort](#sample-initial-response)
- [Beispiel für zweite Anforderung](#sample-second-request) und [Antwort](#sample-second-response)
- [Beispiel für dritte Anforderung](#sample-third-request) und [letzte Antwort](#sample-third-and-final-response)

Nach dem ersten Vorgang wird eine der Nachrichten gelöscht und eine andere als gelesen markiert. Beim [zweiten Synchronisierungsvorgang](#synchronize-messages-in-the-same-folder-in-the-next-round) wird nur das Delta (die Löschung und Aktualisierung) zurückgegeben. Die anderen Nachrichten, die sich nicht geändert haben, werden nicht zurückgegeben.

### <a name="sample-initial-request"></a>Beispiel für ursprüngliche Anforderung

In diesem Beispiel wird der angegebene Ordner zum ersten Mal synchronisiert, sodass die ursprüngliche Synchronisierungsanforderung kein Statustoken enthält. In dieser Runde werden alle Nachrichten in diesem Ordner zurückgegeben.

Die erste Anforderung gibt Folgendes an:

- einen `$select`-Parameter zum Zurückgeben der Eigenschaften `subject`, `sender` und `isRead` für jede Nachricht in der Antwort.
- Den [optionalen Anforderungsheader](#optional-request-header), _odata.maxpagesize_, der gleichzeitig 2 Nachrichten zurückgibt.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a>Beispiel für ursprüngliche Antwort

Die Antwort enthält zwei Nachrichten und einen `@odata.nextLink`-Antwortheader. Die `nextLink`-URL zeigt an, dass weitere abzurufende Nachrichten in dem Ordner vorhanden sind.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "false",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
      "subject": "Holiday promotion sale",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Samantha Booth",
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAVRMKAAAAA=="
    }
  ]
}
```

### <a name="sample-second-request"></a>Beispiel für zweite Anforderung

Die zweite Anforderung gibt die aus der vorherigen Antwort zurückgegebene `nextLink`-URL an. Beachten Sie, dass sie nicht denselben Parameter `$select` wie in der ursprünglichen Anforderung angeben muss, da das `skipToken` in der `nextLink`-URL es codiert und einschließt.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>Beispiel für zweite Antwort

Die zweite Antwort gibt die nächsten 2 Nachrichten in dem Ordner zurück und ein weiteres `nextLink`, was bedeutet, dass weitere abzurufende Nachrichten in dem Ordner vorhanden sind.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlqfdAAAEfYB+\"",
      "subject": "Microsoft Virtual Academy at Contoso",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Elliot Hyde",
          "address": "elliot-hyde@tailspintoys.com"
        }
      },
      "id": "AQMkADNkNAAAgWkAAAA"
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "New or modified user account information",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Randi Welch",
          "address": "randiw@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAgWJAAAA"
    }
  ]
}
```

### <a name="sample-third-request"></a>Beispiel für dritte Anforderung

Die dritte Anforderung verwendet weiterhin die neueste aus der letzten Synchronisierungsanforderung zurückgegebene `nextLink`-URL.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>Beispiel für dritte und letzte Antwort

Die dritte Antwort gibt die einzige in dem Ordner verbleibende Nachricht zurück sowie eine `deltaLink`-URL zurück, was bedeutet, dass die Synchronisierung für diesen Ordner momentan abgeschlossen ist. Speichern und verwenden Sie die `deltaLink`-URL, um [den gleichen Ordner in der nächsten Runde zu synchronisieren](#synchronize-messages-in-the-same-folder-in-the-next-round).

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzFPjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "Fabric CDN now available",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Jodie Sharp",
          "address": "Jodie.Sharp@contoso.com"
        }
      },
      "id": "AAMkADk0MGFkODE3LWEAAA="
    }
  ]
}
```

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a>Synchronisieren der Nachrichten in demselben Ordner im nächsten Vorgang

Mit dem `deltaLink` aus der [letzten Anforderung](#sample-third-request) in der letzten Runde können Sie nur die Nachrichten abrufen, die sich seitdem in diesem Ordner geändert haben (durch Hinzufügung, Löschung oder Aktualisierung). Ihre erste Anforderung in der nächsten Runde sieht folgendermaßen aus, sofern Sie die gleiche maximale Seitengröße in der Antwort beibehalten möchten:

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

Die Antwort enthält ein `deltaLink`. Dies weist darauf hin, dass alle Änderungen im entfernten Nachrichtenordner jetzt synchronisiert sind. Eine Nachricht wurde gelöscht und die andere Nachricht wurde geändert.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS0Dh_6qB-pB2Sa2pUum19a6YAAKnLuxoAAA=",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    }
  ]
}
```

## <a name="see-also"></a>Siehe auch

- [Microsoft Graph-Delta-Abfrage](delta_query_overview.md)
- [Inkrementelle Änderungen an Ereignissen in einer Kalenderansicht abrufen](delta_query_events.md)
- [Inkrementelle Änderungen an Gruppen abrufen](delta_query_groups.md)
- [Inkrementelle Änderungen an Benutzern abrufen](delta_query_users.md)
