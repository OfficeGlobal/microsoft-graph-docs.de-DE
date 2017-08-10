# <a name="update-a-group-setting"></a>Aktualisieren einer Gruppeneinstellung

Aktualisiert die Eigenschaften eines bestimmten Gruppeneinstellungsobjekts.

## <a name="prerequisites"></a>Voraussetzungen

Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*

> Hinweis: Nur Mandantenadministratoren haben die Berechtigungen zum Erstellen, Aktualisieren und Löschen.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->

Aktualisiert eine mandantenweite oder gruppenspezifische Einstellung.

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name | Beschreibung |
|:-----------|:-----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. 

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
| values | settingValue | Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren. |

## <a name="response"></a>Antwort

Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `204 OK` und ein aktualisiertes [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->