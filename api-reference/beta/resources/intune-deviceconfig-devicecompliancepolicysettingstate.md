---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0b98cc4809fb72bb7caf5fe55fe6e912fd00f9b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171498"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|setting|Zeichenfolge|Die gemeldete Einstellung|
|settingName|Zeichenfolge|Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird|
|instanceDisplayName|Zeichenfolge|Name der Einstellungsinstanz, die gemeldet wird.|
|state|[Wurde](../resources/intune-shared-compliancestatus.md)|Der Kompatibilitätsstatus der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
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
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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




