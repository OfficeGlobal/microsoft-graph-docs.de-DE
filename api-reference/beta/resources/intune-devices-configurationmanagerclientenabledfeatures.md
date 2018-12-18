---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
author: tfitzmac
ms.openlocfilehash: e0d704fddc084a455c83c5b55ea9b3911f3f232a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343939"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Im Konfigurations-Manager-Client aktivierte Features
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|inventory|Boolean|Gibt an, ob der Bestand von Intune verwaltet wird|
|modernApps|Boolean|Gibt an, ob die moderne Anwendung von Intune verwaltet wird|
|resourceAccess|Boolean|Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird|
|deviceConfiguration|Boolean|Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird|
|compliancePolicy|Boolean|Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird|
|windowsUpdateForBusiness|Boolean|Gibt an, ob Windows Update for Business von Intune verwaltet wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```





