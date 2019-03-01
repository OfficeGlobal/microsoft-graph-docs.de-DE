---
title: targetResource-Ressourcentyp – Microsoft Graph-API
description: Definiert den komplexen Typ der targetResource-entitätsressource der Microsoft Graph-API, die die Aktivität des Überwachungsprotokoll-Organisations Diensts (Mandanten) unterstützt.
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342289"
---
# <a name="targetresource-resource-type"></a>targetResource-Ressourcentyp

Stellt Ziel Ressourcentypen dar, die der Überwachungsaktivität zugeordnet sind. 


## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Gibt die eindeutige ID der Ressource an.|
|displayName|Zeichenfolge|Gibt den sichtbaren Namen an, der für die Ressource definiert ist. Wird in der Regel bei der Erstellung der Ressource angegeben.|
|type|Zeichenfolge|Beschreibt den Ressourcentyp.  Zu den Beispiel `Application`Werten `Group`gehört `ServicePrincipal`,, `User`und.|
|userPrincipalName|Zeichenfolge|Wenn **Type** auf `User`festgelegt ist, enthält dies den Benutzernamen, der die Aktion initiiert hat; `null` für andere Typen.|
|groupType|Zeichenfolge|Wenn **Type** auf `Group`festgelegt ist, gibt dies den Gruppentyp an.|
|modifiedProperties|[modifiedproperty](modifiedproperty.md) -Auflistung|Gibt den Namen, den alten Wert und den neuen Wert der einzelnen geänderten Attribute an. Eigenschaftswerte sind vom Vorgangstyp abhängig. ****|

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
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String", 
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
