---
title: DefenderCloudBlockLevelType Enum-Typ
description: Mögliche Werte für die Cloud Blockebene
ms.openlocfilehash: 70e43e9659e7dd7be1d3c0a190e21d80d7b8dc41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063651"
---
# <a name="defendercloudblockleveltype-enum-type"></a>DefenderCloudBlockLevelType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für die Cloud Blockebene
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Der Standardwert, verwendet die standardmäßigen Windows Defender Antivirus Blockierung Ebene und bietet starken Erkennung ohne das Risiko von erkennen erhöhen legitime Dateien|
|hohe|1|Besonders weist eine starke Sicherheitsstufe Erkennung.|
|highPlus|2|Hoch + wird die hohe Stufe und Maßnahmen zum Schutz der Addition|
|zeroTolerance|3|0 (null) Toleranz blockiert alle unbekannte ausführbaren Dateien|




