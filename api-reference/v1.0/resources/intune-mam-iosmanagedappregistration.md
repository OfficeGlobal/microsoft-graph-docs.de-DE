---
title: iosManagedAppRegistration-Ressourcentyp
description: Stellt die Synchronisierungsdetails einer iOS-App mit Verwaltungsfunktionen für einen bestimmten Benutzer dar.
ms.openlocfilehash: f62024fe2b3222e1595bfd8fd8c15edb424daff3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016768"
---
# <a name="iosmanagedappregistration-resource-type"></a>iosManagedAppRegistration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|applicationVersion|String|App-Version. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|managementSdkVersion|String|Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|platformVersion|String|Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceType|String|Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceTag|String|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceName|String|Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|flaggedReasons|[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. E.g. Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|userId|String|Benutzer-ID, zu der die App-Registrierung gehört. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|id|String|Schlüssel der Entität Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|Version|String|Version der Entität Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|appliedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|intendedPolicies|Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|Vorgänge|Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden. Geerbt von [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

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
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
