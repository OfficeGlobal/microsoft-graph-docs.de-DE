---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Herunterladen von einer vorherigen version
ms.openlocfilehash: 1d55a457060197cfd9a24a39506003518918d398
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059015"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a>Inhalte einer DriveItemVersion-Ressource herunterladen (Vorschau)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie den Inhalt einer bestimmten Version von einer [DriveItem](../resources/driveitem.md). 

>**Hinweis:** Abrufen des Inhalts der aktuellen Version wird nicht unterstützt. Verwenden Sie stattdessen den [DriveItem Webinhalt-Endpunkt](driveitem-get-content.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |


## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a>Antwort

Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der Bytes der Datei umleitet.

Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.

Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.

## <a name="example"></a>Beispiel

In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a>Antwort

Diese Methode gibt eine Umleitung zurück, über die der Inhalt der Version heruntergeladen werden kann.

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a>Hinweise

OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.

Wenn Ihre app die Liste der verfügbaren Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md) Ressource, die die verfügbare Informationen über die spezielle Version enthält zurückgegeben.

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->