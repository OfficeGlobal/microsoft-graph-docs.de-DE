# <a name="update-page"></a>Seite aktualisieren

Dient zum Aktualisieren des Inhalts einer OneNote-Seite.
## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:   

Notes.ReadWrite oder Notes.ReadWrite.All 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | `Bearer <token>` Ein gültiges OAuth-Token, das der App basierend auf den Anmeldeinformationen des Benutzers und unter der Voraussetzung, dass der Benutzer autorisierten Zugriff hat, bereitgestellt wird. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein Array von [patchContentCommand](../resources/patchcontentcommand.md)-Objekten an, die die Änderungen an der Seite darstellen. Weitere Informationen und Beispiele finden Sie im unter <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote-Seiten aktualisieren</a>.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
