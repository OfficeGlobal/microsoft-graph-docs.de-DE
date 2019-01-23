---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403259"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Ressourcentyp officeClientCheckinStatus

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Entität, die Mandanten Einchecken Stats beschreibt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname des Geräts.|
|deviceName|Zeichenfolge|Name des Aufnahmegeräts einchecken möchten.|
|devicePlatform|Zeichenfolge|Geräteplattform einchecken möchten.|
|devicePlatformVersion|Zeichenfolge|Gerät Plattformversion einchecken möchten.|
|wasSuccessful|Boolean|Wenn das letzte Einchecken erfolgreich war.|
|userId|Zeichenfolge|Benutzer-ID des Geräts.|
|checkinDateTime|DateTimeOffset|Letzte Gerät Einchecken Zeitpunkt in UTC.|
|errorMessage|Zeichenfolge|Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.|
|appliedPolicies|Zeichenfolgenauflistung|Liste der Richtlinien an das Gerät als letzten Checkin übermittelt wurden.|

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



