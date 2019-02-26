---
title: macOsVppAppRevokeLicensesActionResult-Ressourcentyp
description: Definiert Ergebnisse für Aktionen auf MacOS VSS-apps, enthält geerbte Eigenschaften für ActionResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cf8390dc2c1541525e288b81defd073144f4132
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166507"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>macOsVppAppRevokeLicensesActionResult-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definiert Ergebnisse für Aktionen auf MacOS VSS-apps, enthält geerbte Eigenschaften für ActionResult.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userId|Zeichenfolge|Der Aktion zugeordnete UserId.|
|managedDeviceId|Zeichenfolge|Mit der Aktion verknüpfte Geräte-Nr.|
|totalLicensesCount|Int32|Die Anzahl der Lizenzen, für die widerrufen versucht wurde.|
|failedLicensesCount|Int32|Die Anzahl der Lizenzen, für die REVOKE fehlgeschlagen ist.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Der Grund für den Fehlschlagen der Lizenz Widerruf. Mögliche Werte: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|Zeichenfolge|Name der Aktion|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Status der Aktion. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeitpunkt der Einleitung der Aktion|
|lastUpdatedDateTime|DateTimeOffset|Zeitpunkt der letzten Aktualisierung des Aktionszustands|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




