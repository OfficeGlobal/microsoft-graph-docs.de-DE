---
title: Erstellen eines Identitätsanbieters
description: Erstellen eines neuen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a33354c35903fedc3efedb84e9f2ed7bc20c9506
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649413"
---
# <a name="create-identityprovider"></a>Erstellen eines Identitätsanbieters

Erstellen Sie einen neuen [Identitätsanbieter](../resources/identityprovider.md), indem Sie den Anzeigenamen, den Typ des Identitätsanbieters, die Client-ID sowie den geheimen Clientschlüssel angeben.

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
POST /identityProviders
```

## <a name="request-headers"></a>Anforderungsheader

|Name|Beschreibung|
|:---------------|:----------|
|Authorization|Bearer {token}. Erforderlich.|
|Content-Type|application/json. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung des [identityProvider](../resources/identityProvider.md)-Objekts an. Alle in der folgenden Tabelle aufgeführten Eigenschaften sind erforderlich.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|clientId|Zeichenfolge|Die Client-ID für die Anwendung. Dies ist die Client-ID, die Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.|
|clientSecret|Zeichenfolge|Der geheime Clientschlüssel für die Anwendung. Dies ist der geheime Clientschlüssel, den Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.|
|name|Zeichenfolge|Der Anzeigename des Identitätsanbieters.|
|type|Zeichenfolge|Der Typ des Identitätsanbieters. Der Typ muss einer der folgenden Werte für B2C-Szenarien sein: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat</ul>Für B2B kann er nur Google sein.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [identityProvider](../resources/identityProvider.md)-Objekt im Antworttext zurückgegeben. Wenn die Methode nicht erfolgreich ist, wird ein `4xx`-Fehler mit bestimmten Details zurückgegeben.

## <a name="example"></a>Beispiel

Im folgenden Beispiel wird ein **Identitätsanbieter** erstellt.

##### <a name="request"></a>Anforderung

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>Antwort

<!-- { "blockType": "ignored" } -->
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


