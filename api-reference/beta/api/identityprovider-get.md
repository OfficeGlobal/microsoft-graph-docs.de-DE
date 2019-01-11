---
title: Abrufen von identityProvider
description: Abrufen der Eigenschaften einer vorhandenen IdentityProvider.
localization_priority: Normal
ms.openlocfilehash: f0d467bde092f84d092dbcee7c54c01e3ef849f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812971"
---
# <a name="get-identityprovider"></a>Abrufen von identityProvider

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abrufen der Eigenschaften einer vorhandenen [IdentityProvider](../resources/identityprovider.md).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|IdentityProvider.Read.All IdentityProvider.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)| Nicht unterstützt|
|Anwendung|Nicht unterstützt|

Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a>Anforderungsheader

|Name|Beschreibung|
|:---------------|:----------|
|Authorization|Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine JSON-Darstellung der [IdentityProvider](../resources/identityprovider.md) im Antworttext.

## <a name="example"></a>Beispiel

Im folgende Beispiel werden einer bestimmten **IdentityProvider**abgerufen.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
