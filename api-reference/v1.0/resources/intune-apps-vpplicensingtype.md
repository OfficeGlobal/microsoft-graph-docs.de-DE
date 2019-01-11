---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbc52cfd4e14b2010dd133e4fa08e61a30fb63df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814112"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|supportsUserLicensing|Boolescher Wert|Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.|
|supportsDeviceLicensing|Boolescher Wert|Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



