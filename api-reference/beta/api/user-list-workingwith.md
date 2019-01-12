---
title: Liste arbeiten
description: Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f9445dcee294f20f5eadf18cdd648805142c53d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953558"
---
# <a name="list-workingwith"></a>Liste arbeiten

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | User.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
| Header         | Wert                      |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type   | application/json           |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn erfolgreich, gibt diese Methode einen 200 OK-Antwortcode und eine Auflistung von [Benutzerobjekten](../resources/user.md) in der Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
