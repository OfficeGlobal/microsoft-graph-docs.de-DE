---
title: bitLockerRecoveryOptions-Ressourcentyp
description: BitLocker-wiederHerstellungsOptionen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8bbf0db0ca6dd784a47d1bfb5d743ae17695b81
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142112"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>bitLockerRecoveryOptions-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

BitLocker-wiederHerstellungsOptionen.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|Gibt an, ob der zertifikatbasierte Daten Wiederherstellungs-Agent blockiert werden soll.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zum Generieren eines 48-stelligen Wiederherstellungskennworts für den fest-oder Systemdatenträger berechtigt oder erforderlich sind. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Gibt an, ob Benutzer zulässig oder erforderlich sind, um einen 256-Bit-Wiederherstellungsschlüssel für feste oder Systemdatenträger zu generieren. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|hideRecoveryOptions|Boolean|Gibt an, ob das Anzeigen von Wiederherstellungsoptionen im BitLocker-Setup-Assistenten für feste oder Systemdatenträger zugelassen werden soll.|
|enableRecoveryInformationSaveToStore|Boolean|Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS gespeichert werden sollen.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Konfigurieren Sie, welche Teile von BitLocker-Wiederherstellungsinformationen in AD DS gespeichert werden. Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|Gibt an, ob BitLocker aktiviert werden soll, bis Wiederherstellungsinformationen in AD DS gespeichert werden.|

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




