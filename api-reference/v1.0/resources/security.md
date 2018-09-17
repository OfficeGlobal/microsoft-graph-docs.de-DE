# <a name="security-resource-type"></a>Ressourcentyp security

Die Sicherheitsressource ist der Einstiegspunkt für das Objektmodell Sicherheit. Es gibt eine Singleton Sicherheitsressource zurück. Es enthält keine verwendbaren Eigenschaften.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [Warnungen auflisten](../api/alert_list.md) | [alert](alert.md)-Sammlung | Abruf einer Warnungs-Objekt-Sammlung. |
| [get alerts](../api/alert_get.md) | [alert](alert.md)-Sammlung | Abruf eines Warnungs-Objekts. |
| [Aktualisieren von Benachrichtigungen](../api/alert_update.md) | [alert](alert.md)-Sammlung | Abruf eines Warnungs-Objekts. |

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|alerts|[alert](alert.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Beispiel

Die **security**-Ressource ist im Stamm des Diagramms verfügbar.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->