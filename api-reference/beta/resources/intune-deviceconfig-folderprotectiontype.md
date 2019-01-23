---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405716"
---
# <a name="folderprotectiontype-enum-type"></a>FolderProtectionType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für Ordnerschutz

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Gerät Standardwert, keine beabsichtigt.|
|Aktivieren|1|Blockiert Funktionalität.|
|auditMode|2|Ermöglicht die Funktionalität, aber Protokolle zu generieren.|
|blockDiskModification|3|Blockieren von nicht vertrauenswürdigen apps auf Bereiche Datenträger schreiben.|
|auditDiskModification|4|Generieren Sie Protokolle Schreiben von nicht vertrauenswürdigen apps auf Datenträger Bereiche.|




