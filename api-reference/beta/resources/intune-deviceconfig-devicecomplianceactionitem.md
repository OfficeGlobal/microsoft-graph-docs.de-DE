---
title: deviceComplianceActionItem-Ressourcentyp
description: Konfiguration der geplanten Aktivität
ms.openlocfilehash: dc84ee71e6544bf089f3470d607772c2242f7278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060207"
---
# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Welche Aktion erfolgen soll. Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification` und `remoteLock`.|
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




