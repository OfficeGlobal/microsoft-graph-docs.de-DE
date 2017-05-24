# <a name="group-delta"></a>group: delta

Mit einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Um Änderungen an Gruppen zu ermitteln, führen Sie eine Anforderung unter Verwendung der *delta*-Funktion aus. Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).

## <a name="prerequisites"></a>Voraussetzungen

Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.Read.All* oder *Group.ReadWrite.All*

### <a name="http-request"></a>HTTP-Anforderung

Um Änderungen nachzuverfolgen, führe Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Gruppenressource aus. 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a>Abfrageparameter

Beim Nachverfolgen von Änderungen in Gruppen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.

| Abfrageparameter       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen. |

### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt OData-Abfrageparameter zur Anpassung der Antwort.

- Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben. 
- Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Gruppen. 
- Es besteht eingeschränkte Unterstützung für `$orderby`: Der einzige unterstützte `$orderby`-Ausdruck ist `$orderby=receivedDateTime+desc`. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet. 
- `$search` wird nicht unterstützt.

### <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |

### <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben. Die Antwort enthält zudem ein Statustoken, entweder eine nextLink- oder eine deltaLink-URL.

- Wenn eine nextLink-URL zurückgegeben wird, gibt es zusätzliche Seiten mit Daten, die in der Sitzung abgerufen werden müssen. Die Anwendung nimmt weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.

- Wenn eine deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten.

Siehe:</br>
- Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).</br>
- Beispielanforderungen finden Sie unter [Inkrementelle Änderungen für Gruppen abrufen](../../../concepts/delta_query_groups.md).</br>
    
### <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->