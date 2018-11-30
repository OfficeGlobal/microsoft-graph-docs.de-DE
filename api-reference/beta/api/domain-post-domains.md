---
title: Domäne erstellen
description: Fügt eine Domäne zum Mandanten hinzu.
ms.openlocfilehash: d9e6acc2f36e36cfa85bcd35ce13458731f83699
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063058"
---
# <a name="create-domain"></a>Domäne erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Fügt eine Domäne zum Mandanten hinzu.

**Wichtig**: Sie können eine zugeordnete Domäne erst dann mit Ihrem Azure AD-Mandanten verwenden, nachdem der Besitz überprüft wurde. Weitere Informationen finden Sie unter [verificationDnsRecords auflisten](domain-list-verificationdnsrecords.md). Stammdomänen erfordern eine Überprüfung. Beispielsweise muss „contoso.com“ überprüft werden. Wenn eine Stammdomäne überprüft wird, werden Unterdomänen der Stammdomäne automatisch überprüft. Beispielsweise wird „subdomain.contoso.com“ automatisch überprüft, wenn „contoso.com“ überprüft wurde.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.

> Der Anforderungstext enthält die id-Eigenschaft für die neue Domäne. Die id-Eigenschaft ist die einzige Eigenschaft, die angegeben werden kann, und sie ist erforderlich. Der Wert der id-Eigenschaft ist der vollqualifizierte Domänenname, der erstellt werden soll.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/beta/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->