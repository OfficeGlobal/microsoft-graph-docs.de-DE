---
title: Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.
description: Abrufen der Anwendung und Service principal-Objekte mit der angegebenen Richtlinie zugewiesen.
ms.openlocfilehash: 3f281d7c60a506676a78637ad71f1ce26de35e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064579"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie die Objekte [Application](../resources/application.md) und [Service principal](../resources/serviceprincipal.md) mit der angegebenen Richtlinie zugewiesen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` [Code und [Dienstprinzipal](../resources/serviceprincipal.md) und](../resources/application.md) Antwortobjekte im Antworttext. Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.

## <a name="example"></a>Beispiel
Im folgende Beispiel werden die dienstanwendungen und Dienstprinzipale mit einer bestimmten Richtlinie zugewiesen abgerufen.

##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
