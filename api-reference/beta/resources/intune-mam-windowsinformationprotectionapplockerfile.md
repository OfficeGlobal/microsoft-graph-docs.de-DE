---
title: windowsInformationProtectionAppLockerFile-Ressourcentyp
description: Windows Information Protection-AppLocker-Datei
ms.openlocfilehash: 0a6a3117b531f218459287428867d6d38cfd0b6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061111"
---
# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>windowsInformationProtectionAppLockerFile-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Information Protection-AppLocker-Datei
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windowsInformationProtectionAppLockerFiles auflisten](../api/intune-mam-windowsinformationprotectionapplockerfile-list.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekte.|
|[windowsInformationProtectionAppLockerFile abrufen](../api/intune-mam-windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.|
|[windowsInformationProtectionAppLockerFile erstellen](../api/intune-mam-windowsinformationprotectionapplockerfile-create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.|
|[windowsInformationProtectionAppLockerFile löschen](../api/intune-mam-windowsinformationprotectionapplockerfile-delete.md)|Keine|Löscht ein [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt.|
|[windowsInformationProtectionAppLockerFile aktualisieren](../api/intune-mam-windowsinformationprotectionapplockerfile-update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Der Anzeigename|
|fileHash|String|SHA256-Hash der Datei|
|file|Binär|Datei als Bytearray|
|id|String|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```




