# <a name="permanently-delete-item"></a>Element endgültig löschen

Dauerhaftes Löschen eines Elements aus dem Ordner [Gelöschte Elemente](../resources/directory.md).

Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt. Sie können ein Element aus den gelöschten Elementen dauerhaft löschen. Aber nachdem ein Element dauerhaft gelöscht wurde, **kann es nicht** wiederhergestellt werden.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

### <a name="for-users"></a>Für Benutzer:

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadWrite.All, Directory.AccessAsUser.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung | User.ReadWrite.All |

### <a name="for-groups"></a>Für Gruppen:

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All, Directory.AccessAsUser.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Autorisierung  | Bearer&lt;code&gt; *erforderlich*|
| Annehmen  | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->