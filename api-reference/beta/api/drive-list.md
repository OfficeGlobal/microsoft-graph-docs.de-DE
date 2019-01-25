---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Laufwerke auflisten
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 937b537c4ca71b5cee39f60640ede984f1c5797a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517134"
---
# <a name="list-available-drives"></a>Verfügbare Laufwerke auflisten

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie die Liste der [Laufwerk](../resources/drive.md)-Ressourcen ab, die für einen Ziel-Benutzer, eine Ziel-Gruppe oder eine Ziel-[Seite](../resources/site.md) verfügbar sind.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="list-a-groups-drives"></a>Auflisten des Laufwerks einer Gruppe

Für die Auflistung der Dokumentbibliotheken einer Gruppe fordert Ihre App die **drives**-Beziehung bei der Gruppe an.

### <a name="http-request"></a>HTTP-Anforderung

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a>Auflisten der Laufwerke einer Website

Für die Auflistung der Dokumentbibliotheken einer Website fordert Ihre App die **drives**-Beziehung bei der Website an.

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a>Auflisten der Laufwerke eines Benutzers

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a>Die Laufwerke des aktuellen Benutzers auflisten

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Drive](../resources/drive.md)-Objekten im Antworttext zurückgegeben.

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Hinweise

Die meisten Benutzer verfügen nur über eine einzige Laufwerkressource.

Gruppen und Webseiten verfügen möglicherweise über mehrere Laufwerksressourcen.

Laufwerke mit dem [System][]-Facet sind standardmäßig ausgeblendet.
Fügen Sie `system` in Ihre `$select`-Anweisung ein, um sie aufzulisten.

[System]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
