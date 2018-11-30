---
title: Vereinbarung erstellen
description: Erstellen eines neuen Vereinbarung-Objekts.
ms.openlocfilehash: bfcab53b4233d133309c99a4825e184a42670458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059370"
---
# <a name="create-agreement"></a>Vereinbarung erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen eines neuen [Vereinbarung](../resources/agreement.md) -Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Agreement.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|displayName|String|Der Anzeigename der Vereinbarung.|
|isViewingBeforeAcceptanceRequired|Boolesch|Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.|
|Dateien/fileName|String|Name der Datei Vereinbarung (beispielsweise TOU.pdf).|
|Dateien/isDefault|Boolesch|Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kultur die Client-Vorgabe übereinstimmt. Wenn keine der Datei als Standard angegeben ist, wird der ersten als Standard behandelt.|
|Dateien/Sprache|String|Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2. languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet. Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US).|
|Dateien/FileData/data|Binär|Daten, die rechtliche Hinweise das PDF-Dokument darstellt.|

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201, Created` Antwortobjekt Code und [Vereinbarung](../resources/agreement.md) im Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
