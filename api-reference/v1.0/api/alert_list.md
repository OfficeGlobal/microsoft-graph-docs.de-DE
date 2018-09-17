# <a name="list-alerts"></a>Warnungen auflisten

Abrufen einer Liste von [alert](../resources/alert.md)-Objekten.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  SecurityEvents.Read.All, SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.Read.All, SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt folgende [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top` Gibt die aggregierten Top-Ergebnisse von jedem API-Sicherheits-Anbieter zurück.  

Um einen alternativen Eigenschaftensatz zurückzugeben, verwenden Sie die OData `$select` Abfrageparameter, um den Satz von Eigenschaften der **Warnungen** anzugeben, den Sie brauchen.  Wenn z.B. die Eigenschaften **AssignedTo**, **category**und **severity** zurückgegeben werden sollen, dann fügen Sie die Folgendes für Ihre Abfrage ein: `$select=assignedTo,category,severity`.

## <a name="request-headers"></a>Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Autorisierung  | Bearer {code}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an. Der Anforderungstextkörper wird ignoriert.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Sammlung von **alert**-Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
