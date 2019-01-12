---
title: Ressourcentyp bitLockerRecoveryOptions
description: BitLocker Wiederherstellungsoptionen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40ca273b46a1e104afbeac4cbafe967ba76faa22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924839"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Ressourcentyp bitLockerRecoveryOptions

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

BitLocker Wiederherstellungsoptionen.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolescher Wert|Gibt an, ob zertifikatbasierte Datenwiederherstellungsagent blockiert.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zugelassen oder erforderlich, um ein Wiederherstellungskennwort 48 Ziffern generieren für feste oder Systemdatenträger. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zugelassen oder erforderlich, um eine 256-Bit-Wiederherstellungsschlüssel generieren für feste oder Systemdatenträger. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|hideRecoveryOptions|Boolescher Wert|Gibt an, ob Wiederherstellungsoptionen BitLocker-Setup-Assistenten enthält die feste zulassen oder Systemdatenträger.|
|enableRecoveryInformationSaveToStore|Boolescher Wert|Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS speichern können.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Konfigurieren Sie, welche Teile der BitLocker-Wiederherstellungsinformationen in AD DS gespeichert sind. Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boolescher Wert|Gibt an, ob BitLocker aktivieren, bis Wiederherstellungsinformationen in AD DS gespeichert wird.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





