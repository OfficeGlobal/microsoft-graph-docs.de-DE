---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
ms.openlocfilehash: 0c6359d3cb6c776d0f26fdaf88ce7f2f03e5f8c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331717"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Ressourcentyp officeClientCheckinStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die Mandanten Einchecken Stats beschreibt.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userPrincipalName|String|Benutzerprinzipalname des Geräts.|
|deviceName|String|Name des Aufnahmegeräts einchecken möchten.|
|devicePlatform|String|Geräteplattform einchecken möchten.|
|devicePlatformVersion|String|Gerät Plattformversion einchecken möchten.|
|wasSuccessful|Boolesch|Wenn das letzte Einchecken erfolgreich war.|
|userId|String|Benutzer-ID des Geräts.|
|checkinDateTime|DateTimeOffset|Letzte Gerät Einchecken Zeitpunkt in UTC.|
|errorMessage|String|Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.|
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



