# <a name="list-group-settings"></a>Gruppeneinstellungen auflisten

Ruft eine Liste der Gruppeneinstellungsobjekte ab.

## <a name="prerequisites"></a>Anforderungen

Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.Read.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->

Listet mandantenweite oder Gruppeneinstellungen auf.

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.

> Hinweis: $filter wird nicht unterstützt.

## <a name="request-headers"></a>Anforderungsheader
| Name | Beschreibung |
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [groupSetting](../resources/groupsetting.md)-Objekten im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->