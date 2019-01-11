---
title: deviceComplianceActionItem-Ressourcentyp
description: Konfiguration der geplanten Aktivität
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbb67151b38f6c65bf8abae1b16a96b8cb25584f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845808"
---
# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Konfiguration der geplanten Aktivität
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceActionItems auflisten](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekte.|
|[deviceComplianceActionItem abrufen](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.|
|[deviceComplianceActionItem erstellen](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Erstellen eines neuen [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.|
|[deviceComplianceActionItem löschen](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|Keine|Löschen eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[deviceComplianceActionItem aktualisieren](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Aktualisieren der Eigenschaften eines [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|gracePeriodHours|Int32|Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird. Gültige Werte: 0 bis 8760.|
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Welche Aktion erfolgen soll. Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles` und `pushNotification`.|
|notificationTemplateId|String|Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll|
|notificationMessageCCList|Collection von Objekten des Typs „String“|Eine Liste der Gruppen-IDs, die festlegt, wer bei dieser Benachrichtigung auf „CC“ gesetzt wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



