---
title: Erstellen von identityProvider
description: Erstellen einer neuen IdentityProvider durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.
ms.openlocfilehash: 8786cbf6676567a0c6aaef5bf497f50cff1ce9a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062691"
---
# <a name="create-identityprovider"></a>Erstellen von identityProvider

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen einer neuen [IdentityProvider](../resources/identityprovider.md) durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.

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
POST /identityProviders
```

## <a name="request-headers"></a>Anforderungsheader

|Name|Beschreibung|
|:---------------|:----------|
|Authorization|Bearer {token}. Erforderlich.|
|Content-Type|application/json. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [IdentityProvider](../resources/identityprovider.md) -Objekts. Alle in der folgenden Tabelle aufgeführten Eigenschaften sind erforderlich.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|clientId|String|Die Client-ID für die Anwendung. Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.|
|clientSecret|String|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.|
|name|String|Der Anzeigename des Identitätsanbieters.|
|Typ|String|Der Typ der Identität Anbieter. Es muss eine der folgenden Werte sein: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [IdentityProvider](../resources/identityprovider.md) im Antworttext. Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.

## <a name="example"></a>Beispiel

Das folgende Beispiel erstellt eine **IdentityProvider**.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
