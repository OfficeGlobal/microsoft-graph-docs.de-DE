---
title: Ressourcentyp vppTokenRevokeLicensesActionResult
description: Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7044c07b4cc38168219d205f788f4eb8e3eafcf4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928815"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>Ressourcentyp vppTokenRevokeLicensesActionResult

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.

Erbt vom [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Aktionsname Inherited aus [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Status der Aktion Inherited aus [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|startDateTime|DateTimeOffset|Zeit, die die Aktion initiiert wurde, von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) geerbt|
|lastUpdatedDateTime|DateTimeOffset|Aktualisiert der Status der Aktion letzten Inherited [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|totalLicensesCount|Int32|Anzahl der Anzahl der Lizenzen, die widerrufen versucht.|
|failedLicensesCount|Int32|Anzahl der die Anzahl der Lizenzen, die nicht widerrufen werden sollen.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Der Grund für das Revoke Lizenzen-Aktion fehlschlagen. Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.|

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





