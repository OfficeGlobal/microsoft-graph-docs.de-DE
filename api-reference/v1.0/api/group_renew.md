# <a name="group-renew"></a>group: renew

Verlängert den Ablaufzeitraum einer Gruppe. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).
 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All oder Directory.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung | Group.ReadWrite.All oder Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token} |


## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->