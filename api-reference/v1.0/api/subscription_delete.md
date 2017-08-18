# <a name="delete-subscription"></a>Abonnement löschen

Löscht ein Abonnement.

## <a name="prerequisites"></a>Anforderungen

Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.

| Ressourcentyp/Element        | Bereich               |
|-----------------------------|---------------------|
| Kontakte                    | Contacts.Read       |
| Unterhaltungen               | Group.Read.All      |
| Ereignisse                      | Calendars.Read      |
| Nachrichten                    | Mail.Read           |
| Laufwerk (OneDrive eines Benutzers)    | Files.ReadWrite     |
| Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke) | Files.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
