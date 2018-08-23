# <a name="group-delta"></a>group: delta
Mit einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Um Änderungen an Gruppen zu ermitteln, führen Sie eine Anforderung unter Verwendung der *delta*-Funktion aus. Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.Read.All, Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
Um Änderungen nachzuverfolgen, führe Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Gruppenressource aus.

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

## <a name="query-parameters"></a>Abfrageparameter
Beim Nachverfolgen von Änderungen in Gruppen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL.

Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.

In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.

| Abfrageparameter      | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | Zeichenfolge | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | Zeichenfolge | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen. |

### <a name="odata-query-parameters"></a>OData-Abfrageparameter
Diese Methode unterstützt die optionalen OData-Abfrageparameter zur Anpassung der Antwort.

- Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.
- Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Gruppen.
- Es besteht eingeschränkte Unterstützung für `$filter` und `$orderby`:
  * Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`. Sie können mehrere Objekte filtern. Beispiel: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`. Es gilt ein Grenzwert von 50 gefilterten Objekten.
- wird nicht unterstützt.`$search`

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Autorisierung  | Bearer &lt;token&gt;|
| Inhaltstyp  | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben. Die Antwort enthält zudem ein Statustoken, entweder eine nextLink- oder eine deltaLink-URL.

- Wenn eine nextLink-URL zurückgegeben wird, gibt es zusätzliche Seiten mit Daten, die in der Sitzung abgerufen werden müssen. Die Anwendung nimmt weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.

- Wenn eine deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten.

Siehe:</br>
- Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).</br>
- Eine detailliertere Beschreibung finden Sie unter [Abrufen inkrementeller Änderungen für Gruppen](../../../concepts/delta_query_groups.md).</br>

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
>
> Bitte beachten Sie die Eigenschaft *members@delta*, die die ids der Mitgliedsobjekte in dieser Gruppe umfasst.

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
      "mail": "mail-value",
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
    }
  ]
}
```

## <a name="see-also"></a>Siehe auch
- Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).
- Eine detailliertere Beschreibung finden Sie unter [Abrufen inkrementeller Änderungen für Gruppen](../../../concepts/delta_query_groups.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
