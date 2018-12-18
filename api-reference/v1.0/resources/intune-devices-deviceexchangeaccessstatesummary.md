---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
ms.openlocfilehash: dd2784078e8b44b1a02cb5a0013c1e38804912c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301743"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Exchange-Zugriffsstatus für Geräte – Zusammenfassung
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedDeviceCount|Int32|Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.|
|blockedDeviceCount|Int32|Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.|
|quarantinedDeviceCount|Int32|Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.|
|unknownDeviceCount|Int32|Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.|
|unavailableDeviceCount|Int32|Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



