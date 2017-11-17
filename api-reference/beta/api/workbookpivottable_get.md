# <a name="get-workbookpivottable"></a>workbookPivotTable abrufen

Dient zum Abrufen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.

### <a name="prerequisites"></a>Voraussetzungen
Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen: _Files.Read, Files.ReadWrite_

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
### <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

### <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer <code>|
| Arbeitsmappensitzungs-ID  | Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.|

### <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
### <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das  [workbookPivotTable](../resources/workbookpivottable.md)-Objekt im Antworttext zurückgegeben.
### <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/{ver}/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
