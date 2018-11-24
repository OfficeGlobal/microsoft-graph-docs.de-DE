# <a name="group-delta"></a>group: delta
Get neu erstellt, aktualisiert oder Gruppen, einschließlich der Gruppenmitgliedschaft ändert, ohne zum Ausführen eines alles Lesen der ganzen Gruppe-Auflistung gelöscht. Einzelheiten finden Sie unter [Delta-Abfrage verwenden](../../../concepts/delta_query_overview.md) .

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

| Abfrageparameter | Typ  |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen. |

### <a name="odata-query-parameters"></a>OData-Abfrageparameter

Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.

- Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.
- Sie können `$expand=members` mitgliedschaftsänderungen abgerufen.
- Es ist eingeschränkte Unterstützung für `$filter`:
  - Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`. Sie können mehrere Objekte filtern. Beispiel: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Es gilt ein Grenzwert von 50 gefilterten Objekten.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | zurückgeben = minimal <br><br>Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden. Optional. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben. Die Antwort enthält auch ein Status-Token der entweder ein `nextLink` URL oder eine `deltaLink` URL.

- Wenn ein `nextLink` URL zurückgegeben wird:
  - Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen. Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.
  - Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung. Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.

- Wenn ein `deltaLink` URL zurückgegeben wird:
  - Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll. Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.
  - Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung

Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:

- Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.
- Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.
- Wenn die Eigenschaft nicht geändert wurde, den Wert NULL zurück.

> **Hinweis:** Mit dem obigen Verhalten, es ist nicht möglich zur Unterscheidung zwischen einer Eigenschaft, die nicht geändert wurde und eine, die geändert hat eine `null` Wert. Finden Sie im [zweiten Beispiel](#request-2) unten. Wenn dieser Aspekt wichtig ist, sollten das alternative-Verhalten im nächsten Abschnitt beschrieben.

#### <a name="alternative-return-only-the-changed-properties"></a>Alternative: nur die geänderten Eigenschaften zurückgeben

Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:

- Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.
- Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.
- Wenn die Eigenschaft nicht geändert hat, nehmen Sie die Eigenschaft nicht in die JSON-Antwort. (Andere als das Standardverhalten).

> **Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta. Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird. Finden Sie im [dritten Beispiel](#request-3) unten.

### <a name="example"></a>Beispiel

#### <a name="request-1"></a>Anforderung 1

Nachfolgend sehen Sie ein Beispiel der Anforderung. Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a>Antwort 1

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.

>**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
>
> Das Anwesenheitssymbol der *members@delta* -Eigenschaft umfasst die Ids der Member-Objekte in der Gruppe.

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

#### <a name="request-2"></a>Anforderung 2

Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a>Antwort 2

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass `description` und `mailNickname` den Wert der `null` , d. h., die sie möglicherweise nicht geändert oder auf einen leeren Wert festgelegt wurden.

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a>Anforderung 3

Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a>Antwort 3

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass die `mailNickname` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `description` sind enthalten, d. h., deren Werte geändert haben.

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>Siehe auch

- [Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](../../../concepts/delta_query_overview.md).
- [Inkrementelle Änderungen für Gruppen erhalten möchten](../../../concepts/delta_query_groups.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
