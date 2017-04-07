# <a name="get-singlevaluelegacyextendedproperty"></a>singleValueLegacyExtendedProperty abrufen

In diesem Artikel erfahren Sie, wie Sie mithilfe von `$expand` oder `$filter` Ressourceninstanzen abrufen können, die eine einwertige erweiterte Eigenschaft enthalten.

Mit dem Abfrageparameter `$expand` können Sie die angegebene Instanz abrufen, erweitert um die angegebene erweiterte Eigenschaft. Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt.

Mithilfe des Abfrageparameters `$filter` können Sie alle Instanzen der angegebenen Ressource abrufen, die eine erweiterte Eigenschaft haben, deren Eigenschaften **id** und **value** dem festgelegten Filter entsprechen. Der Filter wird auf alle Instanzen der Ressource angewendet, die im Postfach eines angemeldeten Benutzers existieren.

Die folgenden Benutzerressourcen werden unterstützt:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:

- [event](../resources/event.md)-Ressourcen für Gruppen
- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.

## <a name="prerequisites"></a>Voraussetzungen
Zur Ausführung dieser API ist einer der folgenden **Bereiche** erforderlich (je nachdem, welche Ressource Sie abrufen):

- _Mail.Read_
- _Calendars.Read_
- _Contacts.Read_
- _Group.Read.All_ 

## <a name="http-request"></a>HTTP-Anforderung

#### <a name="get-a-resource-instance-using-expand"></a>Abrufen einer Ressourceninstanz mithilfe von `$expand`
Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden.

Abrufen einer **message**-Instanz:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Abrufen einer **mailFolder**-Instanz:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Abrufen einer **event**-Instanz
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Abrufen einer **calendar**-Instanz:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Abrufen einer **contact**-Instanz:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Abrufen einer **contactFolder**-Instanz:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Abrufen einer **event**-Instanz für eine Gruppe:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Abrufen einer **post**-Instanz für eine Gruppe:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a>Abrufen von Ressourceninstanzen mithilfe von `$filter`

Hier sehen Sie, wie Sie alle Instanzen einer unterstützten Ressource abrufen, die eine erweiterte Eigenschaft haben, deren Eigenschaften **id** und **value** dem definierten Filter entsprechen. Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](http://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Vorwärtsschrägstriche und Leerzeichen.


Abrufen von **message**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Abrufen von **mailFolder**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Abrufen von **event**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Abrufen von **calendar**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Abrufen von **contact**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Abrufen von **contactFolder**-Instanzen:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Abrufen von **event**-Instanzen für Gruppen:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Abrufen von **post**-Instanzen für Gruppen:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a>Parameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|_URL parameters_|
|id_value|String|Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.|
|property_value|String|Der Wert der erweiterten Eigenschaft, nach der gefiltert wird. Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt.|

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer <code>|


## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.

#### <a name="get-resource-instance-using-expand"></a>Abrufen von Ressourceninstanzen mithilfe von `$expand`
Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.
  
#### <a name="get-resource-instances-using-filter"></a>Abrufen von Ressourceninstanzen mithilfe von `$filter`
Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die die dem Filter entsprechende erweiterte Eigenschaft enthalten. Der Antworttext enthält nicht die erweiterte Eigenschaft.

## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a>Antwort 1
Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.

Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a>Anforderung 2

Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft haben. Der Filter gibt die erweiterte Eigenschaft zurück, die folgende Merkmale hat:
- Die **id** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).
- Für **value** ist `Green` festgelegt.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a>Antwort 2

Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user_list_messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->