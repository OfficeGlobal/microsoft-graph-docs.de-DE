---
title: mobileAppTroubleshootingAppUpdateHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153641"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a>mobileAppTroubleshootingAppUpdateHistory-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.


Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Zeitpunkt, zu dem das Verlaufselement aufgetreten ist. Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




