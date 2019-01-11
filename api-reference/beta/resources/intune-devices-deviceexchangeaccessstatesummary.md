---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8ca08b026b8e1cdbac4bd0dc73331a9d5df80fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889985"
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





