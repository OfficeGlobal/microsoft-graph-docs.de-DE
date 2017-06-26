# <a name="copy-a-driveitem"></a>DriveItem kopieren

Dient zum Erstellen einer Kopie eines [driveItem](../resources/driveitem.md)-Elements (einschließlich untergeordneter Elemente) unter einem neuen übergeordneten Element oder unter einem neuen Namen.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.


| Name            | Wert                                          | Beschreibung                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Optional.  Verweis auf das übergeordnete Element, in dem die Kopie erstellt wird.                                         |
| name            | string                                         | Optional.  Der neue Name der Kopie. Wenn dieser nicht angegeben wird, wird der gleiche Namen wie für das Original verwendet.    |

**Hinweis:** Das _parentReference_-Element sollte entweder ein `id`- oder `path`-Element enthalten, jedoch nicht beides. Wenn beide enthalten sind, müssen sie auf das gleiche Element verweisen, andernfalls tritt ein Fehler auf.

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a>Antwort

Gibt detaillierte Informationen zum Überwachen des Status der Kopie,bis die Anforderung akzeptiert wird.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a>Bemerkungen

In vielen Fällen wird die Aktion zum Kopieren asynchron durchgeführt. Die Antwort der API gibt nur an, dass der Kopiervorgang akzeptiert oder abgelehnt wurde, wenn der Zieldateiname zum Beispiel bereits verwendet wird.

**Hinweis:** Die API stellt keine Methode zum Abrufen von Informationen dazu bereit, ob die Kopie erfolgreich war.

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
