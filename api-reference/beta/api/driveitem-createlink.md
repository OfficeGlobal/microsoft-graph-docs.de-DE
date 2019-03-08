---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Freigeben einer Datei mit einem Link
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3f119ea285b3fa9e59ec8c67d5a7b3fd304fd196
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480502"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a>Freigabelink für ein DriveItem erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können die Aktion **createLink** verwenden, um ein [DriveItem](../resources/driveitem.md) über einen Freigabelink freizugeben.

Die Aktion **createLink** erstellt einen neuen Freigabelink, falls der angegebene Linktyp für die aufrufende Anwendung noch nicht existiert. Existiert für die App bereits ein Freigabelink des angegebenen Typs, wird dieser bereits vorhandene Freigabelink zurückgegeben.

DriveItem-Ressourcen erben Freigabe-Berechtigungen von ihren Vorgängern.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a>Anforderungstext

Der Anforderungstext definiert die Eigenschaften des Freigabelinks, den Ihre Anwendung anfordert.
Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:

|   Name    |  Typ  |                                 Beschreibung                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| **type**  | string | Der Typ Freigabelink, der erstellt werden soll. Möglich sind `view`, `edit` oder `embed`.       |
| **scope** | Zeichenfolge | Optional. Der Bereich des zu erstellenden Links. Möglich sind `anonymous` oder `organization`. |


### <a name="link-types"></a>Linktypen

Für den Parameter **type** sind die folgenden Werte zulässig:

| Typwert | Beschreibung                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | Erstellt einen schreibgeschützten Link zum DriveItem.                                                        |
| `edit`     | Erstellt einen Link mit Lese-/Schreibzugriff zum DriveItem.                                                       |
| `embed`    | Erstellt einen einbettbaren Link zum DriveItem. Diese Option ist nur für das persönliche OneDrive verfügbar. |

### <a name="scope-types"></a>Bereichstypen

Für den Parameter **scope** sind die nachfolgend aufgeführten Werte zulässig.
Wenn er **scope**-Parameter nicht angegeben ist, wird der Standardlinktyp für die Organisation erstellt.

| Typwert     | Beschreibung                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Erstellt einen Link zum DriveItem, auf das alle über den Link zugreifen können. Anonyme Links können von einem Administrator deaktiviert werden.                 |
| `organization` | Erstellt einen Link zum DriveItem, auf das alle innerhalb der Organisation des Benutzers zugreifen können. Der Linkbereich „organization“ ist nicht für das persönliche OneDrive verfügbar. |

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode eine einzige Ressource des Typs [Permission](../resources/permission.md) im Antworttext zurück. Dabei handelt es sich um die angeforderten Freigabe-Berechtigungen.

Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.

## <a name="example"></a>Beispiel

Im folgende Beispiel wird das Erstellen eines Freigabelinks für das DriveItem angefordert, das durch {ItemId} im OneDrive des Benutzers angegeben wurde.
Der Freigabelink ist schreibgeschützt konfiguriert und kann von allen verwendet werden.

### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a>Antwort

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

OneDrive for Business und SharePoint unterstützen Links, die nur innerhalb eines Unternehmens freigegeben sind.
Diese ähneln anonymen Links, funktionieren aber nur für Mitglieder der Besitzorganisation.
Verwenden Sie den Parameter **scope** mit dem Wert `organization`, um einen Link zu erstellen, der nur innerhalb eines Unternehmens freigegeben ist.

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a>Erstellen von einbettbaren Links

Bei Verwendung des Linktyps `embed` kann der zurückgegebene Wert für „webUrl“ in ein HTML-Element des Typs `<iframe>` eingebettet werden. Wird ein Einbettungslink erstellt, enthält die Eigenschaft `webHtml` den HTML-Code für einen `<iframe>`, der den Inhalt hostet.

**Hinweis:** Einbettungslinks werden nur fürdas persönlich OneDrive unterstützt.

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>HinwBemerkungeneise

* Mit dieser Aktion erstellte Links laufen nicht ab, es sei denn, für die Organisation wird eine Standardablaufrichtlinie erzwungen.
* Links sind in den Freigabeberechtigungen für das Element sichtbar und können von einem Besitzer des Elements entfernt werden.
* Links zeigen immer auf die aktuelle Version eines Elements, es sei denn, das Element ist ausgecheckt (nur SharePoint).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
