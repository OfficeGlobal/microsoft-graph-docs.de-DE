---
title: folderProtectionType-Enumerationstyp
description: Mögliche Werte für den Ordnerschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170336"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für den Ordnerschutz

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Geräte-Standardwert, keine Absicht.|
|Aktivieren|1|Blockieren der Funktionalität.|
|auditMode|2|Funktionalität zulassen, aber Protokolle generieren.|
|blockDiskModification|3|Blockieren Sie nicht vertrauenswürdige apps vor dem Schreiben in Datenträgersektoren.|
|auditDiskModification|4|Generieren von Protokollen, wenn nicht vertrauenswürdige apps in Datenträgersektoren schreiben|




