---
title: deviceComplianceActionItem-Ressourcentyp
description: Konfiguration der geplanten Aktivität
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b0a507ffb080f2354e5c854810554da64b47e7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254688"
---
# <a name="devicecomplianceactionitem-resource-type"></a>deviceComplianceActionItem-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|Schlüssel der Entität|
|gracePeriodHours|Int32|Anzahl Stunden, die gewartet wird, bis die Aktion erzwungen wird. Gültige Werte: 0 bis 8760.|
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Welche Aktion ergriffen werden soll. Mögliche Werte sind: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles` und `pushNotification`.|
|notificationTemplateId|Zeichenfolge|Benachrichtigungs-E-Mail-Vorlage, die verwendet werden soll|
|notificationMessageCCList|String collection|Eine Liste der Gruppen-IDs, die festlegt, wer bei dieser Benachrichtigung auf „CC“ gesetzt wird.|

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



