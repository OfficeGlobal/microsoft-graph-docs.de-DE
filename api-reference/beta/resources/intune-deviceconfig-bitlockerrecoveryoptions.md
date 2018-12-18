---
title: Ressourcentyp bitLockerRecoveryOptions
description: BitLocker Wiederherstellungsoptionen.
author: tfitzmac
ms.openlocfilehash: c85ce3111ed88ce8e8bf54c98d5fd3122571a0be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310605"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Ressourcentyp bitLockerRecoveryOptions

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

BitLocker Wiederherstellungsoptionen.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolesch|Gibt an, ob zertifikatbasierte Datenwiederherstellungsagent blockiert.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zugelassen oder erforderlich, um ein Wiederherstellungskennwort 48 Ziffern generieren für feste oder Systemdatenträger. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zugelassen oder erforderlich, um eine 256-Bit-Wiederherstellungsschlüssel generieren für feste oder Systemdatenträger. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|hideRecoveryOptions|Boolesch|Gibt an, ob Wiederherstellungsoptionen BitLocker-Setup-Assistenten enthält die feste zulassen oder Systemdatenträger.|
|enableRecoveryInformationSaveToStore|Boolesch|Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS speichern können.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Konfigurieren Sie, welche Teile der BitLocker-Wiederherstellungsinformationen in AD DS gespeichert sind. Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boolesch|Gibt an, ob BitLocker aktivieren, bis Wiederherstellungsinformationen in AD DS gespeichert wird.|

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





