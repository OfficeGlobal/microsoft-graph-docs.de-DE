# <a name="update-alert"></a>Update-Benachrichtigung

Aktualisieren Sie eine editierbare **alert**-Eigenschaft innerhalb einer integrierten Lösung, um den Benachrichtigungsstatus und die Zuweisungen zwischen den Lösungen synchron zu halten. Diese Methode aktualisiert jede Lösung, die einen Datensatz der referenzierten alert-ID hat.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |   SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

> **Hinweis:** Bei dieser Methode müssen Sie die **alert** ID als Parameter und „vendorInformation” mit der `provider` und `vendor` angeben.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:-----------|:-----------|
| Autorisierung  | Bearer {code}. Erforderlich.|
|Bevorzugt | zurückgeben = Darstellung |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Request-Body eine JSON-Darstellung der Werte für die relevanten Felder an, die aktualisiert werden sollen. Der Body **muss** die `vendorInformation` Eigenschaft mit gültigen `provider` und `vendor` Feldern enthalten. Die folgende Tabelle listet die Felder auf, die für eine Benachrichtigung aktualisiert werden können. Die Werte für bestehende Eigenschaften, die nicht im Body des Requests enthalten sind, ändern sich nicht. Um die beste Leistung zu erzielen, sollten Sie keine vorhandenen Werte einbeziehen, die sich nicht geändert haben.

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|assignedTo|Zeichenfolge|Name des Analysten, dem die Benachrichtigung für die Selektierung, Untersuchung oder Wartung zugeordnet ist|
|closedDateTime|DateTimeOffset|Zeitpunkt, an dem die Benachrichtigung geschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|comments|String-Sammlung|Analystenkommentare auf die Benachrichtigung (für Kunden- Benachrichtigungsmanagement).|
|Rückmeldung|alertFeedback|Analysten-Feedback auf die Benachrichtigung. Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|Status|alertStatus|Benachrichtigungs-Lebenszyklusstatus (Phase). Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|String-Sammlung|Benutzerdefinierbare Labels, die auf eine Benachrichtigung angewendet werden können und als Filterbedingungen dienen können (z.B. "HVA", "SAW").|
|vendorInformation *|[securityVendorInformation](../resources/securityvendorinformation.md)|Komplexer Typ, der Angaben zum Sicherheitsprodukt/Dienstleister, Anbieter und Unteranbieter enthält (z. B. Lieferant=Microsoft; Anbieter=Windows Defender ATP; Unteranbieter=AppLocker). **Die Felder Anbieter und Lieferant sind Pflichtfelder.**|
(\* Kennzeichnet ein Pflichtfeld.)

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Wird der optionale Anforderungsheader verwendet, gibt die Methode einen `200 OK` Antwortcode und das aktualisierte [alert](../resources/alert.md)-Objekt im Antworttext zurück.

## <a name="example-1"></a>Beispiel 1

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Antwort

Es folgt ein Beispiel für die erfolgreiche Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>Beispiel 2

### <a name="request"></a>Anforderung

Das folgende Beispiel zeigt eine Anforderung, die den `Prefer` Anforderungsheader enthält.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort, wenn der optionale `Prefer: return=representation` Anforderungsheader verwendet wird.

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Alle Eigenschaften werden von einem aktuellen Aufruf zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
