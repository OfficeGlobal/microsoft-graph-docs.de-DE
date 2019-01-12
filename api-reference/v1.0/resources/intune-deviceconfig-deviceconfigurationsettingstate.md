---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68c57b8842136494bf0604a31f62992f7a1c2501
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928010"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Konfigurationseinstellungen für ein bestimmtes Gerät
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|setting|Zeichenfolge|Die gemeldete Einstellung|
|settingName|Zeichenfolge|Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird|
|instanceDisplayName|Zeichenfolge|Name der Einstellungsinstanz, die gemeldet wird.|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|errorCode|Int64|Fehlercode für die Einstellung|
|errorDescription|Zeichenfolge|Fehlerbeschreibung|
|userId|Zeichenfolge|UserId|
|userName|Zeichenfolge|UserName|
|userEmail|Zeichenfolge|UserEmail|
|userPrincipalName|Zeichenfolge|Benutzer-Prinzipalname|
|sources|[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung|Beitragende Richtlinien|
|currentValue|Zeichenfolge|Aktueller Wert der Einstellung auf dem Gerät|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



