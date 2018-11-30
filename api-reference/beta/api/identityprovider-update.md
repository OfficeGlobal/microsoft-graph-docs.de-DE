---
title: IdentityProvider aktualisieren
description: Aktualisieren von Eigenschaften in einer vorhandenen IdentityProvider.
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060841"
---
# <a name="update-identityprovider"></a>IdentityProvider aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren von Eigenschaften in einer vorhandenen [IdentityProvider](../resources/identityprovider.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|IdentityProvider.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)| Nicht unterstützt|
|Anwendung|Nicht unterstützt|

Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>Anforderungsheader

|Name|Beschreibung|
|:---------------|:----------|
|Authorization|Bearer {token}. Erforderlich.|
|Content-Type|application/json. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung ein JSON-Objekt mit einer oder mehrerer Eigenschaften, die aktualisiert werden müssen.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|clientId|String|Die Client-ID für die Anwendung. Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.|
|clientSecret|String|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.|
|name|String|Der Anzeigename des Identitätsanbieters.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.

## <a name="example"></a>Beispiel

Im folgenden Beispiel wird die Definition der Gültigkeitsdauer von token **IdentityProvider** aktualisiert und platziert es als Standard Organisation.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->