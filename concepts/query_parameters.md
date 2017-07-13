# Verwenden von Abfrageparametern zum Anpassen von Antworten
<a id="use-query-parameters-to-customize-responses" class="xliff"></a>

Microsoft Graph stellt optionale Abfrageparameter bereit, die Sie zum Festlegen und Steuern der in einer Antwort zurückgegebenen Datenmenge verwenden können. Die folgenden Abfrageparameter werden unterstützt.

|Name|Beschreibung|Beispiel (klicken Sie auf die Beispiele, um diese im [Graph-Tester][graph-explorer] auszuprobieren)
|:---------------|:--------|:-------|
|[$filter](#filter)|Dient zum Filtern von Ergebnissen (Zeilen).|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$select](#select)|Dient zum Filtern von Eigenschaften (Spalten).|[`/users?$select=givenName,surname`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$expand](#expand)|Dient zum Abrufen von verwandten Ressourcen.|[`/groups/{id}?$expand=members`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/22be6ccb-15a5-459f-94ac-d1393bdd9e66?$expand=members&method=GET&version=v1.0)
|[$orderby](#orderby)|Dient zum Sortieren von Ergebnissen.|[`/users?$orderby=displayName,userPrincipalName desc`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$orderby=displayName,userPrincipalName%20DESC&method=GET&version=v1.0)
|[$top](#top)|Dient zum Beschränken von Ergebnissen. Wird in der Regel mit `$skipToken` verwendet.|[`/users?$top=2`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|Wird zusammen mit `$top` verwendet, um eine Seite von Ergebnissen abzurufen.|Ein Beispiel finden Sie unter `nextLink` in der $top-Abfrage.
|[$count](#count)|Dient zum Abrufen der Gesamtzahl übereinstimmender Ressourcen.|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
<!-- TODO: figure out whether $search is actually used
|[`$search`](#search)|A property and value pair separated by a colon.|
-->

Diese Parameter sind kompatibel mit der [Abfragesprache OData V4][odata-query].

> **Hinweis:** Am `beta`-Endpunkt ist das `$`-Präfix optional. Sie können z. B. `filter` anstelle von `$filter` verwenden. Weitere Informationen und Beispiele finden Sie unter [Abfrageparameter ohne $ Präfixe in Microsoft Graph unterstützen](http://dev.office.com/queryparametersinMicrosoftGraph).

**Codieren von Abfrageparametern:**

Die Werte von Abfrageparametern sollten als Prozentwert codiert werden. Viele HTTP-Clients, Browser und Tools (z. B. der [Graph-Tester][graph-explorer]) sind Ihnen dabei behilflich. Wenn eine Abfrage fehlschlägt, kann eine der möglichen Ursachen dafür sein, dass die Werte von Abfrageparametern nicht ordnungsgemäß codiert wurden.

Eine nicht codierte URL sieht folgendermaßen aus:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Eine korrekt codierte URL sieht folgendermaßen aus:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## filter
<a id="filter" class="xliff"></a>

`$filter` kann verwendet werden, um nur eine Teilmenge einer Auflistung abzurufen. Um beispielsweise Benutzer zu suchen, deren Anzeigename mit `J` beginnt, verwenden Sie `startswith`.

[Ausprobieren im Graph-Tester](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

**Anforderung:**

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

**Antwort:**

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "id": "e013b9f3-a1ab-48d1-907b-e716c39d6363",
            "businessPhones": [
                "4255550100"
            ],
            "displayName": "Jan Madden",
            "givenName": "Jan",
            "jobTitle": null,
            "mail": "demo32@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": "Madden",
            "userPrincipalName": "demo32@a830edad9050849NDA1.onmicrosoft.com"
        },
        {
            "id": "89efe8ed-d141-4151-a3e4-570a70022dff",
            "businessPhones": [
                "+1 425 555 0109"
            ],
            "displayName": "Janet Schorr",
            "givenName": "Janet",
            "jobTitle": "Product Marketing Manager",
            "mail": "janets@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": "18/2111",
            "preferredLanguage": null,
            "surname": "Schorr",
            "userPrincipalName": "janets@a830edad9050849NDA1.onmicrosoft.com"
        },
        ...
    ]
}
```

`$filter` verfügt über eine sehr umfangreiche und aussagekräftige Syntax mit vielen integrierten Operatoren. Logische Operatoren umfassen Gleichheitszeichen (`eq`), Ungleichheitszeichen (`ne`), Zeichen für größer als (`gt`), größer gleich (`gte`), UND (`and`), ODER (`or`), NICHT(`not`) usw. Arithmetische Operatoren umfassen Addieren (`add`), Subtrahieren (`sub`) usw. Zeichenfolgenoperatoren umfassen ENTHÄLT (`contains`), BEGINNT MIT (`startswith`) usw. Lambda-Operatoren umfassen KEINE (`any`) und ALLE (`all`). Weitere Informationen zur `$filter`-Syntax finden Sie im [OData-Protokoll][odata-filter].


## select
<a id="select" class="xliff"></a>

In einer Sammlung oder einer einzelnen Identität verwenden Sie den `$select`-Abfrageparameter, um anstelle der Standardgruppe eine andere Eigenschaftengruppe zum Zurückgeben anzugeben. Der `$select`-Parameter ermöglicht die Auswahl einer Teilmenge oder Obermenge der zurückgegebenen Standardgruppe. Wenn Sie z. B. Ihre Nachrichten abrufen, möchten Sie ggf. festlegen, dass nur die Eigenschaften `from` und `subject` der Nachrichten zurückgegeben werden.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the `name` and `size` properties of items are returned.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name,size
```

By submitting the request with the `$select=name,size` query string, the objects
in the response will only have those property values included.

```json
{
  "value": [
    {
      "id": "13140a9sd9aba",
      "name": "Documents",
      "size": 1024
    },
    {
      "id": "123901909124a",
      "name": "Pictures",
      "size": 1012010210
    }
  ]
}
```-->

## expand
<a id="expand" class="xliff"></a>

In Microsoft Graph-API-Anforderungen wird die Navigation zu einem Objekt oder einer Auflistung des Elements, auf das verwiesen wird, nicht automatisch erweitert. Dies ist beabsichtigt, da der Netzwerkdatenverkehr und die Zeit zum Generieren einer Antwort vom Dienst auf diese Weise reduziert werden. Möglicherweise möchten Sie jedoch in einigen Fällen diese Ergebnisse in eine Antwort einbeziehen.

Sie können den `$expand`-Abfragezeichenfolgen-Parameter verwenden, um die API zum Erweitern eines untergeordneten Objekts oder einer Auflistung und zum Einbeziehen dieser Ergebnisse anzuweisen.

Verwenden Sie beispielsweise zum Abrufen von Stammlaufwerkinformationen und der untergeordneten Elemente auf oberster Ebene in einem Laufwerk den `$expand`-Parameter. In diesem Beispiel wird auch eine [`$select`](#select)-Anweisung verwendet, um nur die Eigenschaften `id` und `name` der untergeordneten Elemente zurückzugeben.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> **Hinweis:** Die maximale Anzahl der erweiterten Objekte für eine Anforderung beträgt 20. Wenn Sie außerdem eine Abfrage für die [`user`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)-Ressource durchführen, können Sie `$expand` zum Abrufen der Eigenschaften von jeweils nur einem untergeordneten Objekt oder einer Auflistung verwenden. Das folgende Beispiel ruft `user`-Objekte ab, jeweils mit bis zu 20 erweiterten `directReport`-Objekten in der `directReports`-Auflistung:

```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```

Einige andere Ressourcen haben möglicherweise ebenfalls einen Höchstwert, führen Sie daher immer eine Überprüfung auf mögliche Fehler durch.

## orderby
<a id="orderby" class="xliff"></a>

Verwenden Sie zum Festlegen der Sortierreihenfolge der aus der Microsoft Graph-API zurückgegebenen Elemente den `$orderby`-Abfrageparameter.

Wenn die zurückgegebenen Benutzer in der Organisation nach dem Anzeigenamen sortiert werden sollen, lautet die Syntax hierfür wie folgt:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

Sie können auch nach komplexen Typentitäten sortieren. Im folgenden Beispiel werden Nachrichten abgerufen und nach dem `address`-Feld der `from`-Eigenschaft sortiert, die vom komplexen Typ `emailAddress` ist:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

Wenn Sie die Ergebnisse in aufsteigender oder absteigender Reihenfolge sortieren möchten, fügen Sie entweder `asc` oder `desc` an den Namen des Felds getrennt durch ein Leerzeichen an, z. B. `?$orderby=name%20desc`.

 > **Hinweis:** Bei Abfragen zur [`user`](../api-reference/v1.0/resources/user.md)-Ressource kann `$orderby` nicht zusammen mit Filterausdrücken verwendet werden.

## top
<a id="top" class="xliff"></a>

Verwenden Sie zum Festlegen der maximalen Anzahl der in einem Resultset zurückzugebenden Elemente den `$top`-Abfrageparameter. Der `$top`-Abfrageparameter ermittelt eine Teilmenge in der Sammlung. Diese Teilmenge setzt sich aus den festgelegten ersten N Elementen zusammen, wobei N eine positive ganze Zahl ist, die durch diesen Abfrageparameter angegeben ist. Wenn beispielsweise die ersten fünf Nachrichten im Postfach des Benutzers zurückgegeben werden sollen, lautet die Syntax wie folgt:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## skip
<a id="skip" class="xliff"></a>

Verwenden Sie zum Festlegen der Anzahl der Elemente, die vor dem Abrufen von Elementen in einer Sammlung übersprungen werden sollen, den `$skip`-Abfrageparameter. Wenn die zurückgegebenen Ereignisse nach Erstellungsdatum sortiert werden, wobei mit dem 21. Ereignis begonnen wird, lautet die Syntax wie folgt.

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## skipToken
<a id="skiptoken" class="xliff"></a>

Verwenden Sie zur Anforderung der zweiten und nachfolgender Seiten mit Graph-Daten den `$skipToken`-Abfrageparameter. Der `$skipToken`-Abfrageparameter wird in URLs bereitgestellt, die von Graph übergeben werden, wenn Graph, in der Regel aufgrund von serverseitigem Paging, einen Teil einer Teilmenge der Ergebnisse zurückgibt. Sie nennt den Punkt in einer Sammlung, an dem der Server das Senden der Ergebnisse beendet hat, und wird zu Graph zurückgegeben, um anzugeben, von wo aus das Senden der Ergebnisse wieder aufgenommen werden sollte. Der Wert eines `$skipToken`-Abfrageparameters könnte z. B. das zehnte Element in einer Sammlung oder das 20. Element in einer Sammlung mit 50 Elementen oder eine andere Position in der Sammlung angeben.

In einigen Fällen wird ein `@odata.nextLink`-Wert angezeigt. Manchmal ist ein `$skipToken`-Wert enthalten. Der `$skipToken`-Wert stellt eine Markierung für den Dienst dar, die angibt, an welcher Stelle das nächste Resultset beginnen soll. Nachfolgend ein Beispiel für einen `@odata.nextLink`-Wert aus einer Antwort, in der Benutzer sortiert nach `displayName` angefordert werden:

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

Um die nächste Seite der Benutzer in Ihrer Organisation zurückzugeben, lautet die Syntax wie folgt.

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## count
<a id="count" class="xliff"></a>

Verwenden Sie `$count` als Abfrageparameter, um die Gesamtzahl der Elemente in einer Sammlung zusammen mit der Seite der Datenwerte anzugeben, die von Graph zurückgegeben werden (siehe folgendes Beispiel):

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

Zurückgegeben werden sowohl die `contacts`-Sammlung als auch die Anzahl der Elemente in der `contacts`-Sammlung in der Eigenschaft `@odata.count`.

>**Hinweis:** Dies wird für [`directoryObject`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject)-Sammlungen nicht unterstützt.

## Suche
<a id="search" class="xliff"></a>

Um die Ergebnisse einer Anforderung zu beschränken, die einem Suchkriterium entsprechen, verwenden Sie den `$search`-Abfrageparameter.

> **Hinweis:** Sie können derzeit **nur** [Nachrichten](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message)- und [Personen](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/person)-Sammlungen suchen. Eine `$search`-Anforderung gibt bis zu 250 Ergebnisse zurück. Sie können [ `$filter` ](#filter) oder [ `$orderby` ](#orderby) nicht in einer Suchabfrage verwenden.

Suchkriterien werden mithilfe von Advanced Query Syntax (AQS) ausgedrückt. Die Ergebnisse sind nach Datum und Uhrzeit sortiert, zu dem bzw. der die Nachricht gesendet wurde.

Sie können die folgenden Eigenschaften in einer `message` in einem `$search`-Kriterium angeben: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`,`toRecipients`

Wenn Sie eine Suche nach Nachrichten durchführen und nur einen Wert angeben, wird die Suche anhand der Standardsucheigenschaften`from`, `subject` und `body` ausgeführt.

Im folgenden Beispiel werden alle Nachrichten im Posteingang des angemeldeten Benutzers zurückgegeben, die das Wort „Pizza“ in einer der drei Standardsucheigenschaften enthalten:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

Im nächsten Beispiel werden alle Nachrichten im Posteingang des Benutzers, die von einer bestimmten E-Mail-Adresse gesendet wurden:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
