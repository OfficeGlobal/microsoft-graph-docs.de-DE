---
title: Ressourcentyp „managedAppRegistration“
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 959bd294ab1752617cea6a6ea5bbe8f0a3802f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869720"
---
# <a name="managedappregistration-resource-type"></a>Ressourcentyp „managedAppRegistration“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|applicationVersion|String|Version der App|
|managementSdkVersion|String|Version des App-Verwaltungs-SDK|
|platformVersion|String|Version des Betriebssystems|
|deviceType|String|Gerätetyp des Hostgeräts|
|deviceTag|Zeichenfolge|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.|
|deviceName|String|Gerätename des Hostgeräts|
|managedDeviceId|Zeichenfolge|Die verwaltete Geräte-ID des Hostgeräts werden soll. Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.|
|azureADDeviceId|Zeichenfolge|Der Azure Active Directory-Gerät Bezeichner des Hostgeräts. Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.|
|deviceModel|Zeichenfolge|Das Gerätemodell für die aktuelle app-Registrierung |
|Einträge deviceManufacturer|Zeichenfolge|Hersteller des Geräts für die aktuelle app-Registrierung |
|flaggedReasons|[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Beispiel: Die App wird auf einem gerooteten Gerät ausgeführt.|
|userId|Zeichenfolge|Benutzer-ID, zu der die App-Registrierung gehört|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner des App-Pakets|
|id|Zeichenfolge|Schlüssel der Entität|
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





