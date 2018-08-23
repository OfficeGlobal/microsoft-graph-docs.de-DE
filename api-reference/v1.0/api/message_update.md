# <a name="update-message"></a>Nachricht aktualisieren

Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Mail.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Mail.ReadWrite    |
|Anwendung | Mail.ReadWrite |

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
| Autorisierung  | Zeichenfolge  | Bearer {token}. Erforderlich. |
| Inhaltstyp | Zeichenfolge  | Die Art der Daten im Textkörper einer Entität. Erforderlich. |
## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|Empfänger|Die BCC-Empfänger der Nachricht. Nur aktualisierbar, wenn isDraft=true.|
|categories|Zeichenfolgenauflistung|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|Recipient collection|Die CC-Empfänger der Nachricht. Nur aktualisierbar, wenn isDraft=true.|
|Von|Empfänger|Der Postfachbesitzer und der Absender der Nachricht. Nur aktualisierbar, wenn isDraft=true. Muss dem tatsächlich verwendeten Posteingang entsprechen.|
|Wichtigkeit|Zeichenfolge|Die Wichtigkeit der Nachricht. Mögliche Werte sind: `Low`, `Normal` und `High`.|
|inferenceClassification | Zeichenfolge | Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind `focused`, oder `other`. |
|internetMessageId |Zeichenfolge |Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. Nur aktualisierbar, wenn isDraft=true.|
|isRead|Boolesch|Gibt an, ob die Nachricht gelesen wurde.|
|replyTo|Recipient collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen. Nur aktualisierbar, wenn isDraft=true.|
|sender|Empfänger|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren. Nur aktualisierbar, wenn isDraft=true und wenn eine Nachricht von einem [geteilten Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) gesendet wird oder wenn die Nachricht im [Auftrag von jemanden](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) gesendet wird. Der Wert muss in jedem Fall dem tatsächlich verwendeten Postfach entsprechen.|
|toRecipients|Recipient collection|Die Empfänger der Nachricht. Nur aktualisierbar, wenn isDraft=true.|
|Text|ItemBody|Der Text der Nachricht. Nur aktualisierbar, wenn isDraft=true.|
|isDeliveryReceiptRequested|Boolesch|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isReadReceiptRequested|Boolesch|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|Betreff|Zeichenfolge|Der Betreff der Nachricht. Nur aktualisierbar, wenn isDraft=true.|

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

## <a name="see-also"></a>Siehe auch

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
