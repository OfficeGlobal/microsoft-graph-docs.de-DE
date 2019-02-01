---
title: Aktualisieren eines Identitätsanbieters
description: Aktualisieren der Eigenschaften eines vorhandenen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b3b945163946586e17e16372523a3349306f77ec
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649404"
---
# <a name="update-identityprovider"></a>Aktualisieren eines Identitätsanbieters

Aktualisieren der Eigenschaften eines vorhandenen [Identitätsanbieters](../resources/identityprovider.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|IdentityProvider.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)| Nicht unterstützt|
|Anwendung|Nicht unterstützt|

Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.

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

Geben Sie im Anforderungstext ein JSON-Objekt mit einer oder mehreren Eigenschaften an, die aktualisiert werden müssen.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|clientId|Zeichenfolge|Die Client-ID für die Anwendung. Dies ist die Client-ID, die Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.|
|clientSecret|Zeichenfolge|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel, den Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.|
|name|Zeichenfolge|Der Anzeigename des Identitätsanbieters.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Wenn die Methode nicht erfolgreich ist, wird ein `4xx`-Fehler mit bestimmten Details zurückgegeben.

## <a name="example"></a>Beispiel

Im folgenden Beispiel wird die Definition der Tokengültigkeitsdauer von **identityProvider** aktualisiert und als Standard in der Organisation festgelegt.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
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
