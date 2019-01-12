---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973751"
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





