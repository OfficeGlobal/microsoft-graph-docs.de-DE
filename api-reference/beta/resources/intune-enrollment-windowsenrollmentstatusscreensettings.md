---
title: Ressourcentyp windowsEnrollmentStatusScreenSettings
description: Registrierung Status Bildschirm Einstellung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978571"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Ressourcentyp windowsEnrollmentStatusScreenSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Registrierung Status Bildschirm Einstellung
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hideInstallationProgress|Boolescher Wert|Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolescher Wert|Zulassen Sie oder blockieren Sie Benutzer für die Verwendung von Gerät vor dem Profil- und app-Installation abgeschlossen|
|blockDeviceSetupRetryByUser|Boolescher Wert|Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen|
|allowLogCollectionOnInstallFailure|Boolescher Wert|Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler|
|customErrorMessage|Zeichenfolge|Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen|
|installProgressTimeoutInMinutes|Int32|Legen Sie die Installation des Fortschritts Timeout in Minuten|
|allowDeviceUseOnInstallFailure|Boolescher Wert|Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler|

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





