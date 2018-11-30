---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
ms.openlocfilehash: fec7290ec559f411bed04e03166b31678d43036f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064830"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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





