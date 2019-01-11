---
title: Abrufen von Einstellungen
description: Lesen Sie Benutzer- und Settings-Objekts.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 30217d43ac453c9e3502b00ece22ac01edf0abfb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852402"
---
# <a name="get-settings"></a>Abrufen von Einstellungen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Lesen Sie Benutzer- und [Settings](../resources/user-settings.md) -Objekts.
Weitere Informationen zum Aktualisieren der Eigenschaften des [Settings](../resources/user-settings.md) -Objekts finden Sie unter [Aktualisieren von benutzereinstellungen](user-update-settings.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read.All, User.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

```http
GET /me/settings/
```

Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All. Weitere Informationen finden Sie unter [Berechtigungen](/graph/permissions-reference).

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Einstellungen](../resources/user-settings.md) im Antworttext.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
