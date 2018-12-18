---
title: Ressourcentyp windowsEnrollmentStatusScreenSettings
description: Registrierung Status Bildschirm Einstellung
author: tfitzmac
ms.openlocfilehash: 8ccf2565d722a09de5f08ebe7333436729ce1b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346928"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Ressourcentyp windowsEnrollmentStatusScreenSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Registrierung Status Bildschirm Einstellung
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hideInstallationProgress|Boolesch|Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolesch|Zulassen Sie oder blockieren Sie Benutzer für die Verwendung von Gerät vor dem Profil- und app-Installation abgeschlossen|
|blockDeviceSetupRetryByUser|Boolesch|Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen|
|allowLogCollectionOnInstallFailure|Boolesch|Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler|
|customErrorMessage|String|Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen|
|installProgressTimeoutInMinutes|Int32|Legen Sie die Installation des Fortschritts Timeout in Minuten|
|allowDeviceUseOnInstallFailure|Boolesch|Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler|

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





