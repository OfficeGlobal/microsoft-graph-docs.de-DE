---
title: mobileAppTroubleshootingAppTargetHistory-Ressourcentyp
description: Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a7171cdde4889ba97a9cd29c4cc8c81ab1a9d58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159353"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a>mobileAppTroubleshootingAppTargetHistory-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verlaufselement, das im Problem Behandlungs Ereignis für Mobile Apps enthalten ist.


Erbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Zeitpunkt, zu dem das Verlaufselement aufgetreten ist. Geerbt von [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|securityGroupId|Zeichenfolge|AAD-Sicherheitsgruppen-ID, auf die Sie gezielt wurde.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status des Elements. Mögliche Werte sind: `unknown`, `success` und `fail`.|
|errorCode|String|Fehlercode für den Fehler, leer, wenn kein Fehler auftritt.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




