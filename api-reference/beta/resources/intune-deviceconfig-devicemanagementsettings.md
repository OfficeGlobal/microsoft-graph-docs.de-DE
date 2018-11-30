---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 81aa176af23451675b58a916e9b092ef119dfcb3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060576"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann. Gültige Werte: 0 bis 120|
|isScheduledActionEnabled|Boolean|Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.|
|secureByDefault|Boolean|Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.|
|enhancedJailBreak|Boolesch|Ist Feature aktiviert ist oder nicht erweiterten Jailbreak Erkennung.|
|deviceInactivityBeforeRetirementInDay|Int32|Wenn das Gerät nicht prüft für die angegebene Anzahl von Tagen, möglicherweise die Mandantendaten entfernt, und das Gerät werden nicht in die Verwaltung. Gültige Werte 30 bis 270|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





