# <a name="update-a-group-setting"></a>Aktualisieren einer Gruppeneinstellung

Mit dieser API können Sie die Eigenschaften des jeweils angegebenen Gruppeneinstellungsobjekts aktualisieren.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              | 
|:--------------------|:---------------------------------------------------------| 
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.ReadWrite.All, Directory.AccessAsUser.All    | 
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    | 
|Anwendung | Directory.ReadWrite.All | 


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