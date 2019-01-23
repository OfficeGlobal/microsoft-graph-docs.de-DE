---
title: Ressourcentyp bitLockerSystemDrivePolicy
description: BitLocker-Verschlüsselung Basis Richtlinien.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425708"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Ressourcentyp bitLockerSystemDrivePolicy

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

BitLocker-Verschlüsselung Basis Richtlinien.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke. Mögliche Werte: sind `aesCbc128`, `aesCbc256`, `xtsAes128` und `xtsAes256`.|
|startupAuthenticationRequired|Boolean|Erfordert zusätzliche Authentifizierung beim Start.|
|startupAuthenticationBlockWithoutTpmChip|Boolean|Gibt an, ob BitLocker ohne kompatibles TPM zulassen (erfordert ein Kennwort oder einen Startschlüssel auf einem USB flash-Laufwerk).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Start zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Startup Pin zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM zum Starten des Schlüssel zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob TPM Start anheften und Schlüssel sind zulässig/erforderlich/nicht zulässig. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|minimumPinLength|Int32|Gibt die minimale Länge des Startup Pin an. Gültige Werte 4 bis 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|BitLocker verschlüsselt Betriebssystemlaufwerke in Abwesenheit der erforderlichen Startup Schlüsselinformationen wiederherstellen können. Diese Einstellung wird angewendet, wenn Sie BitLocker aktivieren.|
|prebootRecoveryEnableMessageAndUrl|Boolean|Aktivieren Sie vor dem Start Recovery Nachrichten- und Url. Wenn RequireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht.|
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




