---
title: bitLockerFixedDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für feste Laufwerke.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e09130a2426f6a7196d472a29f7667b9c044d313
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164295"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>bitLockerFixedDrivePolicy-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

BitLocker-Richtlinien für feste Laufwerke.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Wählen Sie die Verschlüsselungsmethode für feste Laufwerke aus. Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean|Diese Richtlinieneinstellung bestimmt, ob BitLocker-Schutz erforderlich ist, damit feste Datenlaufwerke auf einem Computer schreibbar sind.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Mit dieser Richtlinieneinstellung können Sie steuern, wie mit BitLocker geschützte feste Datenlaufwerke in Abwesenheit der erforderlichen Anmeldeinformationen wiederhergestellt werden. Diese Richtlinieneinstellung wird angewendet, wenn Sie BitLocker aktivieren.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```




