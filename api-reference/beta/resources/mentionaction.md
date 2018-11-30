---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
ms.openlocfilehash: be873ba2b5f9bc1fdd387407c1036435dc6f1fc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061262"
---
# <a name="mentionaction-resource-type"></a>MentionAction-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **MentionAction**-Ressource enthält Informationen zu einer [Aktivität][], in der Personen erwähnt wurden.

[Aktivität]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ                       | Beschreibung
|:--------------|:---------------------------|:-----------------------------
| mentionees    | [IdentitySet][]-Sammlung | Die Identität der in dieser Aktion erwähnten Benutzer.

[identitySet]: identityset.md

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
