---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8238ec075189a138552cb524a22facd99f4d5401
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164267"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann. Gültige Werte: 0 bis 120|
|isScheduledActionEnabled|Boolescher Wert|Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.|
|secureByDefault|Boolean|Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.|
|enhancedJailBreak|Boolescher Wert|Ist Funktion aktiviert oder nicht für eine verbesserte Jailbreak-Erkennung.|
|deviceInactivityBeforeRetirementInDay|Int32|Wenn das Gerät für die angegebene Anzahl von Tagen nicht eincheckt, werden die Unternehmensdaten möglicherweise entfernt, und das Gerät wird nicht verwaltet. Gültige Werte 30 bis 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Der abgeleitete Anmeldeinformationsanbieter, der für dieses Konto verwendet werden soll. Mögliche Werte: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|Zeichenfolge|Der Self-Service-URI des abgeleiteten Anmeldeinformationen Anbieters.|

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
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String"
}
```




