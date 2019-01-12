---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947966"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Ressourcentyp deviceConfigurationTargetedUserAndDevice

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceId|Zeichenfolge|Die Id des Geräts in das Einchecken.|
|deviceName|Zeichenfolge|Der Name des Geräts in das Einchecken.|
|userId|Zeichenfolge|Die Id des Benutzers in das Einchecken.|
|userDisplayName|Zeichenfolge|Der Anzeigename des Benutzers in das Einchecken|
|userPrincipalName|Zeichenfolge|Den UPN des Benutzers in das Einchecken.|
|lastCheckinDateTime|DateTimeOffset|Zeitpunkt der letzten Checkin für diese Benutzer/Geräte-Paar.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





