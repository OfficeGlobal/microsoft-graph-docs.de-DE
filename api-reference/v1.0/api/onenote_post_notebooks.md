# <a name="create-notebook"></a>Notizbuch erstellen

Dient zum Erstellen eines neuen OneNote-[Notizbuchs](../resources/notebook.md).
## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:   

Notes.Create, Notes.ReadWrite oder Notes.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext einen Namen für das Notizbuch an. 

Notizbuchnamen müssen eindeutig sein. Der Name darf nicht mehr als 128 Zeichen und keines der folgenden Zeichen enthalten: ?*\/:<>|'"


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das neue [notebook](../resources/notebook.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->