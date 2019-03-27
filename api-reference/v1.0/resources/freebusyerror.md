---
title: freeBusyError-Ressourcentyp
description: Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.
localization_priority: Normal
ms.openlocfilehash: a08fe8278644ab81f2c1fbe1c7d1530cab27d91b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926604"
---
# <a name="freebusyerror-resource-type"></a>freeBusyError-Ressourcentyp

Stellt Fehlerinformationen aus dem Versuch, die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource zu erhalten.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|message |String |Beschreibt den Fehler. |
|Response Code |Zeichenfolge |Der Antwortcode aus der Abfrage für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
