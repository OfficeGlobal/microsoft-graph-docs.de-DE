---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a387e04b9ebc15d65eb8dd883ecd4a9bae78ad6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969289"
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



