---
title: Ressourcentyp remoteActionAudit
description: Bericht zu remote Aktionen auf den Geräten, die auf einen bestimmten Mandanten gehören initiiert wurden.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7624610ed35a583e0ec11582caa1dccda5ce4ce7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840810"
---
# <a name="remoteactionaudit-resource-type"></a>Ressourcentyp remoteActionAudit

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|String|Berichts-ID|
|deviceDisplayName|String|Name des Aufnahmegeräts Intune.|
|userName|String|\[veraltete\] verwenden Sie stattdessen InitiatedByUserPrincipalName.|
|initiatedByUserPrincipalName|String|Benutzer, der die Aktion Gerät gestartet UPN-Format vorliegt.|
|Aktion|[remoteAction](../resources/intune-devices-remoteaction.md)|Der Name der Aktion. Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Zeit, wenn die Aktion ausgestellt wurde, in UTC angegeben.|
|deviceOwnerUserPrincipalName|String|UPN des Besitzers Gerät.|
|deviceIMEI|String|IMEI des Geräts.|
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





