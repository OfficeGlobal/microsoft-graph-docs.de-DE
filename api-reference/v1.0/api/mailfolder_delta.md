# <a name="mailfolder-delta"></a>mailFolder: delta

Dient zum Abrufen eines Satzes von E-Mail-Ordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.

Ein **delta**-Funktionsaufruf für E-Mail-Ordner in einem Postfach ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](../../../concepts/delta_query_overview.md) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen in den E-Mail-Ordnern abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der E-Mail-Ordner eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal alle E-Mail-Ordner des betreffenden Postfachs vom Server abrufen müssen.

### <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: _Mail.Read_; _Mail.ReadWrite_

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/<id>/mailFolders/delta
```

### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Beim Nachverfolgen von Änderungen in E-Mail-Ordnern wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.

| Abfrageparameter      | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Sammlung von E-Mail-Ordnern zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Sammlung von E-Mail-Ordnern weitere Änderungen zum Nachverfolgen vorliegen. |


#### <a name="odata-query-parameters"></a>OData-Abfrageparameter

Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben. 

### <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type  | string  | application/json. Erforderlich.  |
| Prefer | string  | odata.maxpagesize={x}. Optional. |


### <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [mailFolder](../resources/mailfolder.md)-Sammlungsobjekt im Antworttext zurückgegeben.

### <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von E-Mail-Ordnern im Textkörper der Antwort auf 2 beschränken.

Zum Nachverfolgen von Änderungen in den E-Mail-Ordnern eines Postfachs führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden Statustoken aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen. 

Ein ähnliches Beispiel zeigt, wie die Statustoken zum Nachverfolgen von Änderungen in den Nachrichten eines E-Mail-Ordners verwendet werden: [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md). Die wichtigsten Unterschiede zwischen dem Nachverfolgen von E-Mail-Ordnern und dem Nachverfolgen von Nachrichten in einem Ordner liegen in den Anforderungs-URLs der Delta-Abfrage vor; außerdem geben die Abfrageantworten **mailFolder**- anstelle von **message**-Sammlungen zurück.

<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a>Antwort

Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_  
(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.

Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](../../../concepts/delta_query_overview.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->