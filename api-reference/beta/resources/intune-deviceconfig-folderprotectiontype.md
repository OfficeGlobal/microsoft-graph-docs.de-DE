---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
ms.openlocfilehash: a02f1602f8b9a962124fb7bf2a9731662a6f3057
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061020"
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





