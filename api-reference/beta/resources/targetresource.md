---
title: Ressourcentyp targetResource
description: Gibt eine Auflistung von Ziel Ressourcentypen mit der Aktivität Audit verknüpfte an. Jede Ressource Zieltyp erbt die Eigenschaften dieser Ressource unten beschriebenen.
localization_priority: Normal
ms.openlocfilehash: f86cfe45870292dae93327859c32d38aa2b252fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828679"
---
# <a name="targetresource-resource-type"></a>Ressourcentyp targetResource
Gibt eine Auflistung von Ziel Ressourcentypen mit der Aktivität Audit verknüpfte an. Jede Ressource Zieltyp erbt die Eigenschaften dieser Ressource unten beschriebenen.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge|Gibt den Anzeigenamen der unter Ziel Ressourcentypen unten aufgeführten Ressourcen an.|
|id|Zeichenfolge|Gibt die eindeutige Id der Ressource (zum Beispiel: UserId, AppId, RoleId.).|
|modifiedProperties|[ModifiedProperty](modifiedproperty.md) -Auflistung|Gibt an, Name, alten und neuen Wert der einzelnen Attribute, die geändert. Dies gilt für alle Aktivitäten "Aktualisieren"|

### <a name="target-resource-types"></a>Ziel-Ressourcentypen

Der Ressourcentyp Ziel variiert entsprechend der zugrunde liegenden Ressource:

|Ressourcenname| Referenz|
|-------------|----------|
Gerät|[targetResourceDevice](targetresourcedevice.md)
Verzeichnis|[TargetResourceDirectory] (targetresourcedirectory.md]
Gruppe|[targetResourceGroup](targetresourcegroup.md)
Richtlinie|[targetResourcePolicy](targetresourcepolicy.md)
Rolle|[targetResourceRole](targetresourcerole.md)
Dienstprinzipalnamen|[targetResourceServicePrincipal](targetresourceserviceprincipal.md)
Benutzer|[targetResourceUser](targetresourceuser.md)
Andere|[targetResourceOther](targetresourceother.md)

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
