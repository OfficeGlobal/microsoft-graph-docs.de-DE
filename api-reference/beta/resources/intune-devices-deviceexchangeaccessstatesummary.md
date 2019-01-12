---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49afbb3383035711bc950a9a7226a354ae78f0e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920429"
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





