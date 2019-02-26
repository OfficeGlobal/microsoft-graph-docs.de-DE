---
title: Remote Action Audit-Ressourcentyp
description: Bericht über die Remote Aktionen, die auf den Geräten eingeleitet wurden, die zu einem bestimmten Mandanten gehören.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c06f7472addff7c475eeeb8ac3f1a26cc7ea78bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165877"
---
# <a name="remoteactionaudit-resource-type"></a>Remote Action Audit-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Bericht über die Remote Aktionen, die auf den Geräten eingeleitet wurden, die zu einem bestimmten Mandanten gehören.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[RemoteActionAudits aufListen](../api/intune-devices-remoteactionaudit-list.md)|[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekte.|
|[Remote Action Audit abrufen](../api/intune-devices-remoteactionaudit-get.md)|[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md)|Lesen von Eigenschaften und Beziehungen des [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|
|[Remote Action Audit erstellen](../api/intune-devices-remoteactionaudit-create.md)|[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md)|Erstellen eines neuen [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|
|[Remote Action Audit löschen](../api/intune-devices-remoteactionaudit-delete.md)|Keine|Löscht eine [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md).|
|[Remote Action Audit aktualisieren](../api/intune-devices-remoteactionaudit-update.md)|[Remote Action Audit](../resources/intune-devices-remoteactionaudit.md)|Aktualisieren der Eigenschaften eines [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Berichts-ID.|
|deviceDisplayName|Zeichenfolge|InTune-Gerätename.|
|userName|Zeichenfolge|\[veraltet verwenden\] Sie stattdessen Eigenschaften initiatedbyuserprincipalname.|
|Eigenschaften initiatedbyuserprincipalname|Zeichenfolge|Benutzer, der die Geräte Aktion initiiert hat, Format ist UPN.|
|Aktion|[Remote-Steuerung](../resources/intune-devices-remoteaction.md)|Der Name der Aktion. Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures`,,,,,,,, `factoryResetKeepEnrollmentData`,, `shutDown` ,,,,,, `updateDeviceAccount` `automaticRedeployment` `locateDevice` .|
|requestDateTime|DateTimeOffset|Zeitpunkt der Ausgabe der Aktion in UTC.|
|deviceOwnerUserPrincipalName|Zeichenfolge|UPN des Geräte Besitzers.|
|deviceIMEI|Zeichenfolge|IMEI des Geräts.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Aktionsstatus. Mögliche Werte: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```




