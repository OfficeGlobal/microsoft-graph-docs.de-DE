---
title: Ressourcentyp iosEduDeviceConfiguration
description: iOS Education Gerätekonfiguration
author: tfitzmac
ms.openlocfilehash: 6ec5619f28d75e97080cdea81d547bf0a1a94a2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313587"
---
# <a name="iosedudeviceconfiguration-resource-type"></a>Ressourcentyp iosEduDeviceConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

iOS Education Gerätekonfiguration

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosEduDeviceConfigurations](../api/intune-deviceconfig-iosedudeviceconfiguration-list.md)|[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekte.|
|[Abrufen von iosEduDeviceConfiguration](../api/intune-deviceconfig-iosedudeviceconfiguration-get.md)|[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.|
|[Erstellen von iosEduDeviceConfiguration](../api/intune-deviceconfig-iosedudeviceconfiguration-create.md)|[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|Erstellen eines neuen [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.|
|[IosEduDeviceConfiguration löschen](../api/intune-deviceconfig-iosedudeviceconfiguration-delete.md)|Keines|Löscht eine [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).|
|[IosEduDeviceConfiguration aktualisieren](../api/intune-deviceconfig-iosedudeviceconfiguration-update.md)|[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|teacherCertificateSettings|[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)|Die Trusted Root und PFX-Zertifikate für Lehrer|
|studentCertificateSettings|[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)|Die Trusted Root und PFX-Zertifikate für Schüler|
|deviceCertificateSettings|[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)|Die Trusted Root und PFX-Zertifikate für Geräte|

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
  "@odata.type": "microsoft.graph.iosEduDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  }
}
```





