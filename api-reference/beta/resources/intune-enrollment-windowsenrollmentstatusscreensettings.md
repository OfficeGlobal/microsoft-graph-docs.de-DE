---
title: windowsEnrollmentStatusScreenSettings-Ressourcentyp
description: Einstellung für den Registrierungsstatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684a447b82f285784eda1bf71c13f35d766a570
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148685"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Einstellung für den Registrierungsstatus

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hideInstallationProgress|Boolescher Wert|Anzeigen oder Ausblenden des Installationsfortschritts für den Benutzer|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolescher Wert|Zulassen oder Blockieren des Benutzergeräts vor der vollständigen Profil-und App-Installation|
|blockDeviceSetupRetryByUser|Boolescher Wert|Wiederholen des Setups bei Installationsfehlers für den Benutzer|
|allowLogCollectionOnInstallFailure|Boolescher Wert|Zulassen oder Blockieren der Protokollsammlung bei Installations Ausfällen|
|customErrorMessage|Zeichenfolge|Festlegen der benutzerdefinierten Fehlermeldung beim Installationsfehler|
|installProgressTimeoutInMinutes|Int32|Festlegen des Installationsfortschritts-Timeouts in Minuten|
|allowDeviceUseOnInstallFailure|Boolescher Wert|Zulassen, dass der Benutzer das Gerät bei der Installation weiterhin verwendet|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```




