---
title: officeClientCheckinStatus-Ressourcentyp
description: Entität, die den Eincheckstatus für Mandanten beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156056"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Entität, die den Eincheckstatus für Mandanten beschreibt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname, der das Gerät verwendet.|
|deviceName|Zeichenfolge|Gerätename, der versucht einzuchecken.|
|Deviceplatform wurde|Zeichenfolge|Geräteplattform, die versucht, einzuchecken.|
|devicePlatformVersion|Zeichenfolge|Geräte Plattformversion, die versucht, einzuchecken.|
|wasSuccessful|Boolescher Wert|Wenn das letzte Einchecken erfolgreich war.|
|userId|String|Benutzer-ID, die das Gerät verwendet.|
|checkinDateTime|DateTimeOffset|Zeitpunkt der letzten Geräteüberprüfung in UTC.|
|errorMessage|Zeichenfolge|Fehlermeldung, wenn für das letzte Einchecken verknüpft.|
|appliedPolicies|String collection|Liste der Richtlinien, die beim letzten Einchecken an das Gerät übermittelt wurden.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



