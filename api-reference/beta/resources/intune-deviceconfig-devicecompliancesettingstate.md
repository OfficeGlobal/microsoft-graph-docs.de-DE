---
title: deviceComplianceSettingState-Ressourcentyp
description: Zustand der Gerätekompatibilitätseinstellung für ein bestimmtes Gerät.
ms.openlocfilehash: 4fe524f5a737b5e80201f961a48870cb6e0f0928
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063194"
---
# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zustand der Gerätekompatibilitätseinstellung für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceSettingStates auflisten](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Sammlung|Auflisten der Eigenschaften und Beziehungen der [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekte.|
|[deviceComplianceSettingState abrufen](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.|
|[deviceComplianceSettingState erstellen](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Erstellen eines neuen [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.|
|[deviceComplianceSettingState löschen](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|Keine|Löscht ein [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt.|
|[deviceComplianceSettingState aktualisieren](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|platformType|[deviceType](../resources/intune-shared-devicetype.md)|Gerätetyp-Plattform. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|setting|String|Klassenname und Eigenschaftenname der Einstellung|
|settingName|String|Gemeldeter Einstellungsname|
|deviceId|String|Gemeldete Geräte-ID|
|deviceName|String|Gemeldeter Gerätename|
|userId|String|Gemeldete Benutzer-ID|
|userEmail|String|Gemeldete Benutzer-E-Mail-Adresse|
|userName|String|Gemeldeter Benutzername|
|userPrincipalName|String|Gemeldeter Benutzerprinzipalname|
|deviceModel|String|Gemeldetes Gerätemodell|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```




