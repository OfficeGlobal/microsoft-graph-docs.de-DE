---
title: windowsDomainJoinConfiguration-Ressourcentyp
description: Gerätekonfiguration für Windows-Domänenbeitritt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b0c133a3729098c028139a525c1ae4bdd2b6b75
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152766"
---
# <a name="windowsdomainjoinconfiguration-resource-type"></a>windowsDomainJoinConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Gerätekonfiguration für Windows-Domänenbeitritt.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsDomainJoinConfigurations aufListen](../api/intune-shared-windowsdomainjoinconfiguration-list.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekte.|
|[WindowsDomainJoinConfiguration abrufen](../api/intune-shared-windowsdomainjoinconfiguration-get.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.|
|[WindowsDomainJoinConfiguration erstellen](../api/intune-shared-windowsdomainjoinconfiguration-create.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Erstellen eines neuen [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.|
|[WindowsDomainJoinConfiguration löschen](../api/intune-shared-windowsdomainjoinconfiguration-delete.md)|Keine|Löscht eine [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).|Löscht ein [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekt.|
|[WindowsDomainJoinConfiguration aktualisieren](../api/intune-shared-windowsdomainjoinconfiguration-update.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|**deviceConfiguration**|
|activeDirectoryDomainName|Zeichenfolge|Active Directory-Domänenname, der beitreten soll.|
|computerNameStaticPrefix|Zeichenfolge|Fester Präfix für Computername.|
|computerNameSuffixRandomCharCount|Int32|Dynamisch generierte Zeichen, die als Suffix für den Computernamen verwendet werden. Gültige Werte 3 bis 14|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|organizationalUnit|Zeichenfolge|Organisationseinheit (Organizational Unit, OU), in der das Computerkonto erstellt wird. Wenn dieser Parameter NULL ist, wird der bekannte Computerobjekt Container als veröffentlicht in der Domäne verwendet.|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**deviceConfiguration**|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|networkAccessConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung|Referenz zu den für die Netzwerkkonnektivität erforderlichen Gerätekonfigurationen|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.  Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Antwortobjekte enthalten Eigenschaften, die für den Kontext des Aufrufs relevant sind.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "computerNameStaticPrefix": "String",
  "computerNameSuffixRandomCharCount": 1024,
  "activeDirectoryDomainName": "String"
}
```



