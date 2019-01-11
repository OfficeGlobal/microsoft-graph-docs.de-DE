---
title: Ressourcentyp win32LobAppMsiInformation
description: Enthält die MSI-app-Eigenschaften für eine Win32-App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846515"
---
# <a name="win32lobappmsiinformation-resource-type"></a>Ressourcentyp win32LobAppMsiInformation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die MSI-app-Eigenschaften für eine Win32-App.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|productCode|String|Der MSI-Produktcode.|
|productVersion|String|Der MSI-Version des Produkts.|
|upgradeCode|String|Die MSI-Datei aktualisieren von Code.|
|requiresReboot|Boolean|Gibt an, ob erfordert die MSI-app für den Computer neu starten, um die Installation abzuschließen.|
|packageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|Der Typ des MSI-Paket. Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





