---
title: Ressourcentyp win32LobAppInstallExperience
description: Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74e7dd5b036d42d85e49935f454f3050f604827b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866906"
---
# <a name="win32lobappinstallexperience-resource-type"></a>Ressourcentyp win32LobAppInstallExperience

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Gibt den Typ des Ausführungskontexts, den die app ausgeführt. Mögliche Werte: `system`, `user`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





