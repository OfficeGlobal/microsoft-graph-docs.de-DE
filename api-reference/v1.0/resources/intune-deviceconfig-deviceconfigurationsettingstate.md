---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
ms.openlocfilehash: 056d4e1b501d438feb5bbda6b7910c9998c73cdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017817"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Konfigurationseinstellungen für ein bestimmtes Gerät
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|setting|String|Die gemeldete Einstellung|
|settingName|String|Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird|
|instanceDisplayName|String|Name der Einstellungsinstanz, die gemeldet wird.|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|errorCode|Int64|Fehlercode für die Einstellung|
|errorDescription|String|Fehlerbeschreibung|
|userId|String|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|String|Benutzer-Prinzipalname|
|sources|[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung|Beitragende Richtlinien|
|currentValue|String|Aktueller Wert der Einstellung auf dem Gerät|

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



