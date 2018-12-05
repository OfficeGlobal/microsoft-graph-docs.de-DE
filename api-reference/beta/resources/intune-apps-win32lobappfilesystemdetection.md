---
title: Ressourcentyp win32LobAppFileSystemDetection
description: Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App
ms.openlocfilehash: 914c4f550b480bf16b2048945e66542311653338
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064680"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>Ressourcentyp win32LobAppFileSystemDetection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Datei- oder Ordnerpfads zum Erkennen von einer Win32-App

Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Pfad|String|Der Datei- oder Ordnerpfads zum Erkennen von Win32 Line of Business (LoB)-app|
|fileOrFolderName|String|Der File- oder Folder Name zum Erkennen von Win32 Line of Business (LoB)-app|
|check32BitOn64System|Boolesch|Ein Wert, der angibt, ob diese Datei oder eines Ordners ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|Typ des Dateisystems Erkennung. Mögliche Werte sind: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version` und `sizeInMB`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Der Operator für die Datei oder Fodler Erkennung. Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.|
|detectionValue|String|Der Wert der Erkennung Datei oder eines Ordners|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




