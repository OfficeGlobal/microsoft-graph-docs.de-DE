---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Seite "Veröffentlichen"
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507530"
---
# <a name="sitepage-publish"></a>SitePage: Veröffentlichen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Veröffentlichen Sie die neueste Version einer Ressource [SitePage][] , wodurch die Version der Seite für alle Benutzer verfügbar sind. Wenn die Seite ausgecheckt ist, überprüfen Sie auf der Seite, und veröffentlichen Sie es. Wenn die Seite mit dem Anrufer dieser API aktiviert ist, wird die Seite automatisch eingecheckt und veröffentlicht.

[sitePage]: ../resources/sitepage.md

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
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a>Anforderungstext

Diese Meldung hat keinen Anforderungstext. Alle Anforderungstext gesendet werden ignoriert.

## <a name="response"></a>Antwort

Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
