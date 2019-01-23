---
title: Ressourcentyp windowsEnrollmentStatusScreenSettings
description: Registrierung Status Bildschirm Einstellung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399934"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Ressourcentyp windowsEnrollmentStatusScreenSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Registrierung Status Bildschirm Einstellung

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hideInstallationProgress|Boolean|Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|Zulassen Sie oder blockieren Sie Benutzer für die Verwendung von Gerät vor dem Profil- und app-Installation abgeschlossen|
|blockDeviceSetupRetryByUser|Boolean|Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen|
|allowLogCollectionOnInstallFailure|Boolean|Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler|
|customErrorMessage|Zeichenfolge|Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen|
|installProgressTimeoutInMinutes|Int32|Legen Sie die Installation des Fortschritts Timeout in Minuten|
|allowDeviceUseOnInstallFailure|Boolean|Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler|

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




