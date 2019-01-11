---
title: Ressourcentyp keyCredential
description: Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist. Die **KeyCredentials** -Eigenschaft der Anwendung und ServicePrincipal Entitäten ist eine Auflistung von **KeyCredential**.
localization_priority: Normal
ms.openlocfilehash: 0319568dad271f13b396d2f75a71839e85c96c40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851562"
---
# <a name="keycredential-resource-type"></a>Ressourcentyp keyCredential

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält eine wichtige Anmeldeinformationen eine Anwendung oder einen Dienstprinzipal zugeordnet ist. Die **KeyCredentials** -Eigenschaft der [Anwendung](application.md) und [ServicePrincipal](serviceprincipal.md) Entitäten ist eine Auflistung von **KeyCredential**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binär| Benutzerdefinierte Schlüssel-ID |
|endDateTime|DateTimeOffset|Datum und Uhrzeit, zu der die Anmeldeinformationen abläuft. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Schlüssel-ID|Guid|Der eindeutige Bezeichner (GUID) für den Schlüssel.|
|startDateTime|DateTimeOffset|Datum und Uhrzeit, an dem die Anmeldeinformationen gültig ist. Der Zeitstempeltyp stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|type|String|Die Art der wichtigsten Anmeldeinformationen. beispielsweise "Symmetrisch".|
|Verwendung|String|Eine Zeichenfolge, die den Zweck beschreibt, für den der Schlüssel verwendet werden kann. beispielsweise "Überprüfen".|
|Key|Binär|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
