---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Seite "Veröffentlichen"
localization_priority: Normal
ms.openlocfilehash: 0b98f22dda2c4b08d04150b8b24126fdff5ca505
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836155"
---
# <a name="sitepage-publish"></a>SitePage: Veröffentlichen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
