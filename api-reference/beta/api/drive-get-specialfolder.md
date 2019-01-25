---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Spezielle Ordner abgerufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fb7afa57093cf4ab1587654c840098deeceb0c24
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514593"
---
# <a name="get-a-special-folder-by-name"></a>Speziellen Ordner nach Name abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwenden Sie spezielle Auflistung, um auf einen speziellen Ordner basierend auf dem Namen zuzugreifen.

Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner in OneDrive, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin nach diesem Ordner gesucht werden.

Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.

> **Hinweis:**  Wenn Sie nur über Leseberechtigungen verfügen und einen speziellen Ordner anfordern, der nicht vorhanden ist, wird ein `403 Forbidden`-Fehler angezeigt.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|            Berechtigungstyp             |                                           Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                            |
| Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |
| Anwendung                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                                                         |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a>Namen für spezielle Ordner

Im Folgenden sind Namen für spezielle Ordner aufgelistet, die in OneDrive und OneDrive for Business zur Verfügung stehen.

| Name        | Ordner-ID    | Beschreibung                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Dokumente   | `documents`  | Der Ordner „Dokumente“.                                                    |
| Fotos      | `photos`     | Der Ordner „Fotos“.                                                       |
| Eigene Aufnahmen | `cameraroll` | Der Sicherungsordner für Eigene Aufnahmen.                                           |
| Anwendungsstamm    | `approot`    | Der persönliche Ordner der Anwendung. In der Regel unter `/Apps/{Application Name}` |
| Musik       | `music`      | Der Ordner „Musik“.                                                        |


### <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von `$expand` und `$select` zur Anpassung der Antwort.

## <a name="response"></a>Antwort

Die Methode gibt den Antwortcode `200 OK` und das aktualisierte [driveItem](../resources/driveitem.md)-Objekt im Antworttext zurück.

Sie können diese Methode der Adressierung eines speziellen Ordners mit dem zusätzlichen Aufruf der Eigenschaften oder Beziehungen auf das DriveItem anwenden.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a>Abrufen der untergeordneten Elemente eines speziellen Ordners

Um die untergeordneten Elemente eines speziellen Ordners anzufordern, können Sie die `children`-Sammlung anfordern oder die Option [expand](/graph/query-parameters) verwenden, um die Sammlung untergeordneter Elemente zu erweitern.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

> **Hinweis:** DriveItems mit der `specialFolder`-Facette geben an, dass das Element ein spezieller Ordner ist und der Zugriff über die `special`-Sammlung erfolgen kann.

Wenn Ihre App über Leseberechtigungen verfügt, schläft die Anforderung zum Abrufen eines speziellen Ordners oder der untergeordneten Elemente eines speziellen Ordners mit dem Fehler `404 Not Found` oder `403 Forbidden` fehl, wenn der spezielle Ordner nicht bereits vorhanden ist.

<!--
{
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-get-specialfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
