---
title: androidPermissionAction-Ressourcentyp
description: Zuordnung zwischen einer Android-App-Berechtigung und der Aktion, die Android ausführen sollte, wenn diese Berechtigung angefordert wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e00bb351f2eff093dee21cb393ba622bc5e29ea9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161572"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Zuordnung zwischen einer Android-App-Berechtigung und der Aktion, die Android ausführen sollte, wenn diese Berechtigung angefordert wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Berechtigung|Zeichenfolge|Android-Berechtigungszeichenfolge, definiert in der offiziellen Android-Dokumentation.  Beispiel "Android. Permission. READ_CONTACTS".|
|Aktion|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Typ der Android-Berechtigungs Aktion. Mögliche Werte sind: `prompt`, `autoGrant` und `autoDeny`.|

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




