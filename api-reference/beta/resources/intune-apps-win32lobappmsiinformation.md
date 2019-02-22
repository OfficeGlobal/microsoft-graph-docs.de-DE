---
title: win32LobAppMsiInformation-Ressourcentyp
description: Enthält Eigenschaften der MSI-App für eine Win32-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f330111a3e924e54cf23c30cd98d20e85cb38022
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158646"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften der MSI-App für eine Win32-app.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|productCode|Zeichenfolge|Der MSI-Produktcode.|
|productVersion|Zeichenfolge|Die MSI-Produktversion.|
|upgradeCode|Zeichenfolge|Der MSI-UpgradeCode.|
|requiresReboot|Boolescher Wert|Gibt an, ob für die MSI-App der Computer neu gestartet werden muss, um die Installation abzuschließen.|
|PackageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|Der MSI-Pakettyp. Mögliche Werte sind: `perMachine`, `perUser` und `dualPurpose`.|
|productName|String|Der MSI-Produktname.|
|publisher|Zeichenfolge|Der MSI-Herausgeber.|

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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```




