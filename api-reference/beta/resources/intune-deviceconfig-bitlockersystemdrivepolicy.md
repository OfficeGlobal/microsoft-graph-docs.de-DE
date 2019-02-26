---
title: bitLockerSystemDrivePolicy-Ressourcentyp
description: BitLocker-Verschlüsselungs Basisrichtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27b4492dd6df2821cfdeb885d3412536c0d3991c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164890"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>bitLockerSystemDrivePolicy-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

BitLocker-Verschlüsselungs Basisrichtlinien.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Wählen Sie die Verschlüsselungsmethode für Betriebssystemlaufwerke aus. Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Boolean|Zusätzliche Authentifizierung beim Start erforderlich.|
|startupAuthenticationBlockWithoutTpmChip|Boolean|Gibt an, ob BitLocker ohne kompatibles TPM zugelassen werden soll (erfordert ein Kennwort oder einen Systemstartschlüssel auf einem USB-Flashlaufwerk).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob der TPM-Start zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob die TPM-Start Pin zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob der TPM-Startschlüssel zulässig/erforderlich/nicht zulässig ist. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob die TPM-Start-PIN und der Schlüssel zulässig/erforderlich/nicht zulässig sind. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|minimumPinLength|Int32|Gibt die minimale Länge der Start-PIN an. Gültige Werte 4 bis 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Ermöglicht die Wiederherstellung von BitLocker-verschlüsselten Betriebssystemlaufwerken, wenn die erforderlichen Startschlüssel Informationen fehlen. Diese Richtlinieneinstellung wird angewendet, wenn Sie BitLocker aktivieren.|
|Prebootrecoveryenablemessageandurl wurden|Boolean|Aktivieren Sie die Vorabstart-Wiederherstellungs Nachricht und-URL. Wenn requireStartupAuthentication auf false festgelegt ist, wirkt sich dieser Wert nicht aus.|
|prebootRecoveryMessage|Zeichenfolge|Definiert eine benutzerdefinierte Wiederherstellungs Nachricht.|
|prebootRecoveryUrl|Zeichenfolge|Definiert eine benutzerdefinierte Wiederherstellungs-URL.|

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




