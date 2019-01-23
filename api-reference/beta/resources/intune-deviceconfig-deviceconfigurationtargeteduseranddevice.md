---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410742"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Ressourcentyp deviceConfigurationTargetedUserAndDevice

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




