# <a name="move-a-driveitem"></a>DriveItem-Element verschieben

Zum Verschieben eines DriveItem-Elements zu einem neuen übergeordneten Element fordert die App die Aktualisierung von **ParentReference** des zu verschiebenden DriveItem-Elements an. Dies ist ein Sonderfall der [Update](item_update.md)-Methode. Die App kann das Verschieben eines Elements zu einem neuen Container und das Aktualisieren anderer Eigenschaften des Elements in einer einzigen Anforderung verbinden.

Elemente können mit dieser Anforderung nicht zwischen [Laufwerken](../resources/drive.md)  verschoben werden.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All


## <a name="http-request"></a>HTTP-Anforderung

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Typ   | Beschreibung                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben. |


## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext den neuen Wert für die **parentReference**-Eigenschaft an. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

**Hinweis:** Die `"id:" "root"`-Syntax kann nicht beim Verschieben von Elementen in den Stammordner einer OneDrive-Umgebung verwendet werden. Sie müssen entweder die echte ID des Stammordners oder `{"path": "/drive/root"}` für die übergeordnete Referenz verwenden.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
In diesem Beispiel wird ein durch {item-id} angegebenes Element in den Ordner **Dokumente** in der OneDrive-Umgebung des Benutzers verschoben.

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
