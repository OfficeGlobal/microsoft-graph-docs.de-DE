---
title: vppTokenRevokeLicensesActionResult-Ressourcentyp
description: Der Status der Aktion REVOKE Licenses, die für das Apple Volume Purchase Program-Token ausgeführt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3ccf2bfd72ae9f6aeb85e3a7228faac09a8b2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158170"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Der Status der Aktion REVOKE Licenses, die für das Apple Volume Purchase Program-Token ausgeführt wurde.


Erbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) geerbter Aktionsname|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Status der von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)geerbten Aktion. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeitpunkt, zu dem die Aktion initiiert wurde, geerbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Zeitpunkt, zu dem der Aktionsstatus zuletzt aktualisiert wurde, geerbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|totalLicensesCount|Int32|Die Anzahl der zu wider rufenden Lizenzen.|
|failedLicensesCount|Int32|Die Anzahl der Lizenzen, die nicht widerrufen werden konnten.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Der Grund für den Fehlschlagen der Lizenz Widerruf. Mögliche Werte: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




