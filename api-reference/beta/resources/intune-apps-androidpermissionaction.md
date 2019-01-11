---
title: Ressourcentyp androidPermissionAction
description: Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: daf72bbc5f8d1e32480adeda72c3f759255f54db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860536"
---
# <a name="androidpermissionaction-resource-type"></a>Ressourcentyp androidPermissionAction

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Berechtigung|String|In der Dokumentation zu offiziellen Android definierte Zeichenfolge Android Berechtigung.  Beispiel für 'android.permission.READ_CONTACTS'.|
|Aktion|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Typ der Berechtigung Android-Aktion. Mögliche Werte sind: `prompt`, `autoGrant` und `autoDeny`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





