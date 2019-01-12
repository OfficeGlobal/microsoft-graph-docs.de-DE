---
title: Ressourcentyp iosVppAppRevokeLicensesActionResult
description: Ergebnisse für Aktionen auf iOS Apps Vpp definiert, geerbte Eigenschaften für ActionResult enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 13bc69a0c04eb7b9742f6c549fd1ae976cf25561
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986992"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>Ressourcentyp iosVppAppRevokeLicensesActionResult

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ergebnisse für Aktionen auf iOS Apps Vpp definiert, geerbte Eigenschaften für ActionResult enthält.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userId|Zeichenfolge|Benutzer-ID der Aktion zugeordnet.|
|managedDeviceId|Zeichenfolge|Geräte-ID der Aktion zugeordnet.|
|totalLicensesCount|Int32|Anzahl der Anzahl der Lizenzen, die für die Revoke versucht wurde.|
|failedLicensesCount|Int32|Anzahl der Anzahl von Lizenzen für welche Revoke ist fehlgeschlagen.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Der Grund für das Revoke Lizenzen-Aktion fehlschlagen. Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.|
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
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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





