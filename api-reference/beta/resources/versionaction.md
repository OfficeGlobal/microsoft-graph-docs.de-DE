---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
ms.openlocfilehash: f22761dd713b6d09d5e6fafb765d6d43bfc81bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060073"
---
# <a name="versionaction-resource-type"></a>VersionAction-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wenn die **VersionAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität eine neue Version erstellt hat.

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | Der Name der neuen Version, die von dieser Aktion erstellt wurde.

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
