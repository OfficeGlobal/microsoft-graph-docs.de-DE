---
title: 'domain: verify'
description: Überprüft den Besitz der Domäne.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be1eb96647fe78a9a796703ea67004f8fa4571cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972495"
---
# <a name="domain-verify"></a>domain: verify

Überprüft den Besitz der Domäne.

> **Wichtig:** Gilt nur für nicht überprüfte Domänen. Bei einer nicht überprüften Domäne hat die Eigenschaft „isVerified“ des [domain](../resources/domain.md)-Objekts den Wert „false“.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.Read.All, Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "id": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
