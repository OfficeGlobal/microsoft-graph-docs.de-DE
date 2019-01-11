---
title: sharedPCAccountManagerPolicy-Ressourcentyp
description: SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c8e66f64f316b0fd0a31ab17d143e3da2375ee4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856602"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>sharedPCAccountManagerPolicy-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

SharedPC-Konto-Manager-Richtlinie. Gilt nur, wenn der Konto-Manager aktiviert ist.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|accountDeletionPolicy|[sharedPCAccountDeletionPolicyType](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|Konfiguriert, wann Konten gelöscht werden. Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.|
|cacheAccountsAboveDiskFreePercentage|Int32|Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden. Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat. Gültige Werte: 0 bis 100.|
|inactiveThresholdDays|Int32|Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat. Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.|
|removeAccountsBelowDiskFreePercentage|Int32|Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben. Konten, die am längsten inaktiv waren, werden zuerst gelöscht. Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat. Gültige Werte: 0 bis 100.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```





