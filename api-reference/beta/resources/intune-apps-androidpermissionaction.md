---
title: Ressourcentyp androidPermissionAction
description: Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425631"
---
# <a name="androidpermissionaction-resource-type"></a>Ressourcentyp androidPermissionAction

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Zuordnung zwischen einer Android-app-Berechtigung und die Aktion Android sollte verwenden, wenn diese Berechtigung angefordert wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Berechtigung|Zeichenfolge|In der Dokumentation zu offiziellen Android definierte Zeichenfolge Android Berechtigung.  Beispiel für 'android.permission.READ_CONTACTS'.|
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




