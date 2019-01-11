---
title: Ressourcentyp macOSTrustedRootCertificate
description: Vertrauenswürdige Stammzertifikat für OS X Konfigurationsprofil.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c7c39be9a4c09b5235ef10e17eab3c0bbfac2f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851408"
---
# <a name="macostrustedrootcertificate-resource-type"></a>Ressourcentyp macOSTrustedRootCertificate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Vertrauenswürdige Stammzertifikat für OS X Konfigurationsprofil.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste macOSTrustedRootCertificates](../api/intune-deviceconfig-macostrustedrootcertificate-list.md)|[MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Auflistung|Listeneigenschaften und Beziehungen der [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekte.|
|[Abrufen von macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-get.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Lesen Sie Eigenschaften und Beziehungen des [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekts.|
|[Erstellen von macOSTrustedRootCertificate](../api/intune-deviceconfig-macostrustedrootcertificate-create.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Erstellen eines neuen [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekts.|
|[MacOSTrustedRootCertificate löschen](../api/intune-deviceconfig-macostrustedrootcertificate-delete.md)|Keine|Löscht eine [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).|
|[MacOSTrustedRootCertificate aktualisieren](../api/intune-deviceconfig-macostrustedrootcertificate-update.md)|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Aktualisieren Sie die Eigenschaften eines [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|trustedRootCertificate|Binär|Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.|
|Aus|String|Der Dateiname in der Benutzeroberfläche angezeigt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "trustedRootCertificate": "binary",
  "certFileName": "String"
}
```





