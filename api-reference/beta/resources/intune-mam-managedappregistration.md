---
title: Ressourcentyp „managedAppRegistration“
description: Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung. Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63645c7817281f201fd66e39e7fac2c59ff88f5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151121"
---
# <a name="managedappregistration-resource-type"></a>Ressourcentyp „managedAppRegistration“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.
Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „managedAppRegistration](../api/intune-mam-managedappregistration-list.md)|Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.|
|[Abrufen von „managedAppRegistration“](../api/intune-mam-managedappregistration-get.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Funktion „getUserIdsWithFlaggedAppRegistration“](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|String-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst|
|applicationVersion|Zeichenfolge|Version der App|
|managementSdkVersion|Zeichenfolge|Version des App-Verwaltungs-SDK|
|platformVersion|Zeichenfolge|Version des Betriebssystems|
|deviceType|Zeichenfolge|Gerätetyp des Hostgeräts|
|deviceTag|Zeichenfolge|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.|
|deviceName|Zeichenfolge|Gerätename des Hostgeräts|
|managedDeviceId|Zeichenfolge|Die ID des verwalteten Geräts des Hostgeräts. Der Wert kann auch dann leer sein, wenn das Host Gerät verwaltet wird.|
|azureADDeviceId|String|Die Azure Active Directory-Geräte-ID des Hostgeräts. Der Wert kann auch dann leer sein, wenn das Host Gerät Azure Active Directory registriert ist.|
|deviceModel|Zeichenfolge|Das Gerätemodell für die aktuelle App-Registrierung |
|deviceManufacturer|Zeichenfolge|Der Gerätehersteller für die aktuelle App-Registrierung |
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Beispiel: Die App wird auf einem gerooteten Gerät ausgeführt.|
|userId|String|Benutzer-ID, zu der die App-Registrierung gehört|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner des App-Pakets|
|id|string|Schlüssel der Entität|
|Version|Zeichenfolge|Version der Entität|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|appliedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde|
|intendedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat|
|operations|Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




