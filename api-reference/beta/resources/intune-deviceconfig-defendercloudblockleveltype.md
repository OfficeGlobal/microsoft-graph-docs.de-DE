---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
author: tfitzmac
ms.openlocfilehash: c58c844097c18ff86beaef4a0e48d9b8a39043f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317444"
---
# <a name="defendercloudblockleveltype-enum-type"></a>DefenderCloudBlockLevelType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für die Cloud Blockebene
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien|
|hohe|1|Besonders weist eine starke Sicherheitsstufe Erkennung.|
|highPlus|2|Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition|
|zeroTolerance|3|0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien|





