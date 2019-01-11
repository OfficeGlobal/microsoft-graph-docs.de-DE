---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ff75c5d73db35c5c2ff70ad3a3dc3e4509745188
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825233"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Ressourcentyp officeClientCheckinStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die Mandanten Einchecken Stats beschreibt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname des Geräts.|
|deviceName|Zeichenfolge|Name des Aufnahmegeräts einchecken möchten.|
|devicePlatform|Zeichenfolge|Geräteplattform einchecken möchten.|
|devicePlatformVersion|Zeichenfolge|Gerät Plattformversion einchecken möchten.|
|wasSuccessful|Boolescher Wert|Wenn das letzte Einchecken erfolgreich war.|
|userId|Zeichenfolge|Benutzer-ID des Geräts.|
|checkinDateTime|DateTimeOffset|Letzte Gerät Einchecken Zeitpunkt in UTC.|
|errorMessage|Zeichenfolge|Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.|
|appliedPolicies|Collection von Objekten des Typs „String“|Liste der Richtlinien an das Gerät als letzten Checkin übermittelt wurden.|

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



