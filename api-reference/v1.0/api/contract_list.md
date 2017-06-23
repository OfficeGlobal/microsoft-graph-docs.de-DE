# <a name="list-contracts"></a>Verträge auflisten

Dient zum Abrufen einer Liste von [contract](../resources/contract.md)-Objekten, die einem Partnermandanten zugeordnet sind.

### <a name="prerequisites"></a>Voraussetzungen

Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.Read.All*, *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*.

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort. 

> Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.

### <a name="request-headers"></a>Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

### <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.

### <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->