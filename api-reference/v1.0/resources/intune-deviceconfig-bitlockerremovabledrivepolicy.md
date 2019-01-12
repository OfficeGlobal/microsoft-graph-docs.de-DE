---
title: bitLockerRemovableDrivePolicy-Ressourcentyp
description: BitLocker-Richtlinien für Wechseldatenträger.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 040f4230cf1d3aab02f97237b88093126f8dc24c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926337"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a>bitLockerRemovableDrivePolicy-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

BitLocker-Richtlinien für Wechseldatenträger.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Wählen Sie die Verschlüsselungsmethode für Wechseldatenträger aus. Mögliche Werte: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean|Gibt an, ob der Schreibzugriff auf in einer anderen Organisation konfigurierte Geräte blockiert wird.  Wenn „requireEncryptionForWriteAccess“ auf „false“ gesetzt ist, wirkt sich dieser Wert nicht aus.|
|blockCrossOrganizationWriteAccess|Boolean|Diese Richtlinieneinstellung bestimmt, ob der BitLocker-Schutz erforderlich ist, damit Wechseldatenträger auf einem Computer beschreibbar sind.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



