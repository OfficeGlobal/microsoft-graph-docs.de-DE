---
title: Ressourcentyp win32LobAppRegistryDetection
description: Enthält Registrierungseigenschaften zum Erkennen von einer App Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23362d7613d198bdd848205cbf20944e9a592f04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923901"
---
# <a name="win32lobappregistrydetection-resource-type"></a>Ressourcentyp win32LobAppRegistryDetection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Registrierungseigenschaften zum Erkennen von einer App Win32

Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|check32BitOn64System|Boolescher Wert|Ein Wert, der angibt, ob in diesem Registrierungspfad ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system|
|keyPath|Zeichenfolge|Registrierungsschlüsselpfad zum Erkennen von Win32 Line of Business (LoB)-app|
|Wertname|Zeichenfolge|Der Name des Registrierungsschlüssels|
|detectionType|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Der Erkennung Datentyp. Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Der Operator für die Registrierung Daten Erkennung. Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.|
|detectionValue|Zeichenfolge|Den Registrierungswert Erkennung|

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





