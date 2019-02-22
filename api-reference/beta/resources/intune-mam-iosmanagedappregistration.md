---
title: iosManagedAppRegistration-Ressourcentyp
description: Stellt die Synchronisierungsdetails einer iOS-App mit Verwaltungsfunktionen für einen bestimmten Benutzer dar. Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2bb5f864c61d5a9f9b12fee5eb62dae844bb266
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169223"
---
# <a name="iosmanagedappregistration-resource-type"></a>iosManagedAppRegistration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt die Synchronisierungsdetails einer iOS-App mit Verwaltungsfunktionen für einen bestimmten Benutzer dar.
Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.


Erbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosManagedAppRegistrations auflisten](../api/intune-mam-iosmanagedappregistration-list.md)|[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) auf.|
|[iosManagedAppRegistration abrufen](../api/intune-mam-iosmanagedappregistration-get.md)|[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)|Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|applicationVersion|Zeichenfolge|App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|managementSdkVersion|Zeichenfolge|Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|platformVersion|Zeichenfolge|Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceType|Zeichenfolge|Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceTag|Zeichenfolge|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceName|Zeichenfolge|Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|managedDeviceId|Zeichenfolge|Die ID des verwalteten Geräts des Hostgeräts. Der Wert kann auch dann leer sein, wenn das Host Gerät verwaltet wird. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|azureADDeviceId|String|Die Azure Active Directory-Geräte-ID des Hostgeräts. Der Wert kann auch dann leer sein, wenn das Host Gerät Azure Active Directory registriert ist. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceModel|Zeichenfolge|Das Gerätemodell für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceManufacturer|Zeichenfolge|Der Gerätehersteller für die aktuelle App-Registrierung, geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Beispiel: Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|userId|String|Benutzer-ID, zu der die App-Registrierung gehört. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|id|string|Schlüssel der Entität Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|appliedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|intendedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|operations|Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




