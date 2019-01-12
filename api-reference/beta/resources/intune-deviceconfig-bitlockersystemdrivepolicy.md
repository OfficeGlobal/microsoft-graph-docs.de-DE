---
title: Ressourcentyp bitLockerSystemDrivePolicy
description: BitLocker-Verschlüsselung Basis Richtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28c3b597f25e7ea83577c18620280885f4149dcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924657"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Ressourcentyp bitLockerSystemDrivePolicy

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

BitLocker-Verschlüsselung Basis Richtlinien.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke. Mögliche Werte: sind `aesCbc128`, `aesCbc256`, `xtsAes128` und `xtsAes256`.|
|startupAuthenticationRequired|Boolescher Wert|Erfordert zusätzliche Authentifizierung beim Start.|
|startupAuthenticationBlockWithoutTpmChip|Boolescher Wert|Gibt an, ob BitLocker ohne kompatibles TPM zulassen (erfordert ein Kennwort oder einen Startschlüssel auf einem USB flash-Laufwerk).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Start zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Startup Pin zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM zum Starten des Schlüssel zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Start anheften und Schlüssel sind zulässig/erforderlich/nicht zulässig. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|minimumPinLength|Int32|Gibt die minimale Länge des Startup Pin an. Gültige Werte 4 bis 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|BitLocker verschlüsselt Betriebssystemlaufwerke in Abwesenheit der erforderlichen Startup Schlüsselinformationen wiederherstellen können. Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.|
|prebootRecoveryEnableMessageAndUrl|Boolescher Wert|Aktivieren Sie vor dem Start Recovery Nachrichten- und Url. Wenn RequireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht.|
|prebootRecoveryMessage|Zeichenfolge|Definiert eine benutzerdefinierte Wiederherstellung Nachricht.|
|prebootRecoveryUrl|Zeichenfolge|Definiert eine benutzerdefinierte Wiederherstellung-URL.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```





