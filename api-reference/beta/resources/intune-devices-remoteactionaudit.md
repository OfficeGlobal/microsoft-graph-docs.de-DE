---
title: Ressourcentyp remoteActionAudit
description: Bericht zu remote Aktionen auf den Geräten, die auf einen bestimmten Mandanten gehören initiiert wurden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404911"
---
# <a name="remoteactionaudit-resource-type"></a>Ressourcentyp remoteActionAudit

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Bericht zu remote Aktionen auf den Geräten, die auf einen bestimmten Mandanten gehören initiiert wurden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Auflistung|Listeneigenschaften und Beziehungen der [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekte.|
|[Abrufen von remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Lesen Sie Eigenschaften und Beziehungen des [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|
|[Erstellen von remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Erstellen eines neuen [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|
|[RemoteActionAudit löschen](../api/intune-devices-remoteactionaudit-delete.md)|Keine|Löscht eine [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[RemoteActionAudit aktualisieren](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Aktualisieren Sie die Eigenschaften eines [RemoteActionAudit](../resources/intune-devices-remoteactionaudit.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Berichts-ID|
|deviceDisplayName|Zeichenfolge|Name des Aufnahmegeräts Intune.|
|userName|Zeichenfolge|\[veraltete\] verwenden Sie stattdessen InitiatedByUserPrincipalName.|
|initiatedByUserPrincipalName|Zeichenfolge|Benutzer, der die Aktion Gerät gestartet UPN-Format vorliegt.|
|Aktion|[remoteAction](../resources/intune-devices-remoteaction.md)|Der Name der Aktion. Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Zeit, wenn die Aktion ausgestellt wurde, in UTC angegeben.|
|deviceOwnerUserPrincipalName|Zeichenfolge|UPN des Besitzers Gerät.|
|deviceIMEI|Zeichenfolge|IMEI des Geräts.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Status der Aktion. Mögliche Werte: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|

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




