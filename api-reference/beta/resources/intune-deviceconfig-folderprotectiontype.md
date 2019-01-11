---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 435f3ea01f5a8ffc3c4cb54034d415d54732db5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826131"
---
# <a name="folderprotectiontype-enum-type"></a>FolderProtectionType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für Ordnerschutz
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Gerät Standardwert, keine beabsichtigt.|
|Aktivieren|1|Blockiert Funktionalität.|
|auditMode|2|Ermöglicht die Funktionalität, aber Protokolle zu generieren.|
|blockDiskModification|3|Blockieren von nicht vertrauenswürdigen apps auf Bereiche Datenträger schreiben.|
|auditDiskModification|4|Generieren Sie Protokolle Schreiben von nicht vertrauenswürdigen apps auf Datenträger Bereiche.|





