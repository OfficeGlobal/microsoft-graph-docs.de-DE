---
title: PasswordCredential Ressourcentyp
description: Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält. Die **PasswordCredentials** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **PasswordCredential**.
ms.openlocfilehash: 79d3f76606533cf639f52ed22cd93f353e18e977
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058227"
---
# <a name="passwordcredential-resource-type"></a>PasswordCredential Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Anwendung oder ein Dienst Prinzipal zugeordnete Kennwort Anmeldeinformationen enthält. Die **PasswordCredentials** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **PasswordCredential**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binär|            |
|endDateTime|DateTimeOffset|Datum und Uhrzeit, an dem das Kennwort läuft ab. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Schlüssel-ID|Guid|            |
|startDateTime|DateTimeOffset|Datum und Uhrzeit, an dem das Kennwort gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|secretText|String| Die Kennwörter müssen 16-64 Zeichen lang sein. |
|Hinweis|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
