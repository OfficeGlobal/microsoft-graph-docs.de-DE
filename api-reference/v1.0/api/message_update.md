# <a name="update-message"></a>Nachricht aktualisieren

Dient zum Aktualisieren der Eigenschaften des Nachrichtenobjekts.
## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.ReadWrite*
## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type | string  | Die Art der Daten im Textkörper einer Entität. Erforderlich. |
## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|Die Bcc:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|Recipient collection|Die Cc:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|Von|Recipient|Der Postfachbesitzer und der Absender der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|Wichtigkeit|String|Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.|
|inferenceClassification | String | Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`. |
|internetMessageId |String |Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. Kann nur aktualisiert werden, wenn IsDraft = True.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|replyTo|Recipient collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen. Kann nur aktualisiert werden, wenn IsDraft = True.|
|sender|Recipient|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren. Kann nur aktualisiert werden, wenn IsDraft = True.|
|toRecipients|Recipient collection|Die An:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|body|ItemBody|Der Text der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|subject|String|Der Betreff der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.|

Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
