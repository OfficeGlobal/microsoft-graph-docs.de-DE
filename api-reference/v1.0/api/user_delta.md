# <a name="user-delta"></a>user: delta

Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht. Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](../../../concepts/delta_query_overview.md) .

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | User.Read, User.ReadWrite    |
|Anwendung | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

Um Änderungen nachzuverfolgen, führen Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Benutzerressource aus.

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>Abfrageparameter

Nachverfolgen von Änderungen in Benutzer verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe. Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben. Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.

Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.

In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.

| Abfrageparameter      | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| $deltatoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.|
| $skiptoken | string | Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen. |

### <a name="odata-query-parameters"></a>OData-Abfrageparameter

Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.

- Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.
- Es ist eingeschränkte Unterstützung für `$filter`:
  - Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`. Sie können mehrere Objekte filtern. Beispiel: `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Es gilt ein Grenzwert von 50 gefilterten Objekten.

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | zurückgeben = minimal <br><br>Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden. Optional. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

### <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/user.md) -Auflistungsobjekt in der Antworttext. Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.

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
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a>Antwort 1

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a>Anforderung 2

Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>Antwort 2

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass `jobTitle` und `mobilePhone` den Wert der `null` , d. h., die sie möglicherweise nicht geändert oder auf einen leeren Wert festgelegt wurden.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a>Anforderung 3

Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>Antwort 3

Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen. Beachten Sie, dass die `mobilePhone` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `jobTitle` sind enthalten, d. h., deren Werte geändert haben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- [Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](../../../concepts/delta_query_overview.md).
- [Inkrementelle Änderungen für Benutzer erhalten möchten](../../../concepts/delta_query_users.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->