# <a name="create-a-sharing-link-for-a-driveitem"></a>Freigabelink für ein DriveItem erstellen

Sie können die Aktion **createLink** verwenden, um ein [DriveItem](../resources/driveitem.md) über einen Freigabelink freizugeben.

Die Aktion **createLink** erstellt einen neuen Freigabelink, falls der angegebene Linktyp für die aufrufende Anwendung noch nicht existiert. Existiert für die App bereits ein Freigabelink des angegebenen Typs, wird dieser bereits vorhandene Freigabelink zurückgegeben.

Ressourcen des Typs „DriveItem“ erben Berechtigungen von ihren Vorgängern.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

  * Files.ReadWrite

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a>Anforderungstext
Der Anforderungstext definiert den Typ des Freigabelinks, nach dem die Anwendung sucht. Die Anforderung sollte ein JSON-Objekt mit dieser Eigenschaft sein.

| Name      | Typ   | Beschreibung                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| **type**  | string | Der Typ Freigabelink, der erstellt werden soll. Möglich sind `view`, `edit` oder `embed`.       |
| **scope** | string | Der Bereich des zu erstellenden Links. Möglich sind `anonymous` oder `organization`. Optional. |

## <a name="link-types"></a>Linktypen
Für den Parameter **type** sind die folgenden Werte zulässig:

| Typwert | Beschreibung                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | Erstellt einen schreibgeschützten Link zum Element.                                                        |
| `edit`     | Erstellt einen Lese-/Schreiblink zum Element.                                                       |
| `embed`    | Erstellt einen einbettbaren Link zum Element. Diese Option ist nur für OneDrive Personal verfügbar. |

## <a name="scope-types"></a>Bereichstypen
Für den Parameter **scope** sind die nachfolgend aufgeführten Werte zulässig. Der Parameter ist optional. Wird der Parameter **scope** nicht festgelegt, wird von den verfügbaren Links derjenige mit den meisten Berechtigungen erstellt.

| Typwert     | Beschreibung                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Erstellt einen Link zum Element, auf den jedermann zugreifen kann. Anonyme Links können vom Mandantenadministrator deaktiviert werden.                 |
| `organization` | Erstellt einen Link zum Element, auf den innerhalb einer Organisation zugegriffen werden kann. Der Linkbereich „organization“ ist nicht für OneDrive Personal verfügbar. |

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode eine einzige Ressource des Typs [Permission](../resources/permission.md) im Antworttext zurück. Dabei handelt es sich um die Berechtigung für den angeforderten Freigabelink.

Der Dienst prüft zuerst die aktuellen Berechtigungen, um festzustellen, ob für die aufrufende Anwendung bereits eine Berechtigung mit demselben Wert für den Parameter **type** existiert.

Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.

##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>Erstellen von nur innerhalb eines Unternehmens freigegebenen Links

OneDrive for Business und SharePoint unterstützen Links, die nur innerhalb eines Unternehmens freigegeben sind. Diese ähneln anonymen Links, funktionieren aber nur für Mitglieder des Mandanten, der Besitzer ist. Verwenden Sie den Parameter **scope** mit dem Wert `organization`, um einen Link zu erstellen, der nur innerhalb eines Unternehmens freigegeben ist.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a>HTTP-Antwort

Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a>Einbettbare Links

Bei Verwendung des Linktyps `embed` kann der zurückgegebene Wert für „webUrl“ in ein HTML-Element des Typs `<iframe>` eingebettet werden. Wird ein Einbettungslink erstellt, enthält die Eigenschaft `webHtml` den HTML-Code für einen `<iframe>`, der den Inhalt hostet.

**Hinweis:** Einbettungslinks werden nur für Ressourcen des Typs [Drive](../resources/drive.md) unterstützt, bei denen für **driveType** `personal` festgelegt ist.

## <a name="remarks"></a>Bemerkungen

* Mit dieser Aktion erstellte Links laufen nicht ab, es sei denn, für die Organisation wird eine Standardablaufrichtlinie erzwungen.
* Links sind in den Freigabeberechtigungen für das Element sichtbar und können von einem Besitzer des Elements entfernt werden.
* Links zeigen immer auf die aktuelle Version eines Elements, es sei denn, das Element ist ausgecheckt (nur SharePoint).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
