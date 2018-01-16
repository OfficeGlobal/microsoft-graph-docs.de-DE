# <a name="list-messages"></a>Nachrichten auflisten

Mit dieser Methode können Sie die Nachrichten im Postfach des angemeldeten Benutzers abrufen (einschließlich der Nachrichten aus den Ordnern „Gelöschte Elemente“ und „Clutter“).

Zurzeit gibt dieser Vorgang Nachrichtentext ausschließlich im HTML-Format zurück.


### <a name="get-messages-in-another-users-message-folder"></a>Anzeigen von Nachrichten im Nachrichtenordner eines anderen Benutzers

Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Nachrichten aus dem Nachrichtenordner eines anderen Benutzers anzeigen. Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.

Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John. Der Benutzer Garth hat einen Nachrichtenordner für John freigegeben. Sie können die Nachrichten in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

Diese Funktion gilt für alle unterstützten GET-Nachrichtenvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten). Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.

Wenn Garth weder seinen Nachrichtenordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Nachrichten aus dem Nachrichtenordner eines angemeldeten Benutzers anzuzeigen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

Diese Funktion ist nur in GET-Vorgängen verfügbar für:

- Freigegebene Kontaktordner, Kalender und Nachrichtenordner 
- Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern
- Die oben aufgeführten Ressourcen in delegierten Postfächern

Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.Read, Mail.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Mail.Read, Mail.ReadWrite    |
|Anwendung | Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung

So rufen Sie alle Nachrichten in einem Benutzerpostfach ab:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

So rufen Sie Nachrichten in einem spezifischen Ordner in einem Benutzerpostfach ab:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Besser: outlook.body-content-type | string | Das Format, in der die **body**- und **uniqueBody**-Eigenschaften zurückgegeben werden sollen. Werte können „Text“ oder „html“ sein. Wenn die Kopfzeile nicht angegeben ist, werden die **body**- und **uniqueBody**-Eigenschaften im HTML-Format zurückgegeben. Optional. |


## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Message](../resources/message.md)-Objekten im Antworttext zurückgegeben.

Die Standardseitengröße für diese Anforderung liegt bei 10 Nachrichten.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
