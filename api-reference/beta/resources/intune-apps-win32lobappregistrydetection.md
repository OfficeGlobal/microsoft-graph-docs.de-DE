---
title: Ressourcentyp win32LobAppRegistryDetection
description: Enthält Registrierungseigenschaften zum Erkennen von einer App Win32
author: tfitzmac
ms.openlocfilehash: 5adeca1b569531d15657acc2a8960bab60580dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347740"
---
# <a name="win32lobappregistrydetection-resource-type"></a>Ressourcentyp win32LobAppRegistryDetection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Registrierungseigenschaften zum Erkennen von einer App Win32

Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|check32BitOn64System|Boolesch|Ein Wert, der angibt, ob in diesem Registrierungspfad ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system|
|keyPath|String|Registrierungsschlüsselpfad zum Erkennen von Win32 Line of Business (LoB)-app|
|Wertname|String|Der Name des Registrierungsschlüssels|
|detectionType|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Der Erkennung Datentyp. Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Der Operator für die Registrierung Daten Erkennung. Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.|
|detectionValue|String|Den Registrierungswert Erkennung|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





