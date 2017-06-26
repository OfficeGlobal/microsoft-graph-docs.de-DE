# <a name="update-schemaextension"></a>schemaExtension aktualisieren

Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen [schemaExtension](../resources/schemaextension.md).

Die Aktualisierung gilt für alle Ressourcen, die in der Eigenschaft **targetTypes** der Erweiterung enthalten sind. Diese Ressourcen gehören zu den [unterstützenden Ressourcentypen](../../../concepts/extensibility_overview.md#supported-resources).

Nur die App, mit der eine Schemaerweiterung erstellt wurde (Besitzer-App), kann additive Aktualisierungen an der Erweiterung vornehmen, wenn die Erweiterung den Status **InDevelopment** oder **Available** aufweist. Dies bedeutet, dass die App keine benutzerdefinierten Eigenschaften oder Zielressourcentypen aus der Definition entfernen kann. Die App kann jedoch die Beschreibung der Erweiterung ändern.

## <a name="prerequisites"></a>Voraussetzungen

Der folgende **Bereich** ist erforderlich, um diese API auszuführen: *Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

### <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type   | application/json | 

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Beschreibung für die Schemaerweiterung.|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung|Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden. Nur additive Änderungen sind zulässig. |
|status|String|Der Lebenszyklusstatus der Schemaerweiterung. Bei der Erstellung ist der anfängliche Status **InDevelopment**. Mögliche Statusübergänge sind von **InDevelopment** zu **Available**, von **Available** zu **Deprecated** und von **Deprecated** zu **Available**.|
|targetTypes|String collection|Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->