---
title: recipient-Ressourcentyp
description: 'Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar. '
localization_priority: Normal
ms.openlocfilehash: 89d1ae7703d5b8b0e2a94027e74fbd4c4ebf9ed8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875292"
---
# <a name="recipient-resource-type"></a>recipient-Ressourcentyp

Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar. 

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|emailAddress|[EmailAddress](emailaddress.md)|Die E-Mail-Adresse des Empfängers.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
