---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
ms.openlocfilehash: 7669caa27be93786d381266f88b41ae456314bb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065917"
---
# <a name="windowsupdatetype-enum-type"></a>WindowsUpdateType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Welche Geräte Branch erhält ihre Updates aus
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|all|1|Semikolons jährlichen Channel (Ziel). Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.|
|businessReadyOnly|2|Semikolons jährlichen Channel. Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.|
|windowsInsiderBuildFast|3|Erstellen von Windows-Insider - Fast|
|windowsInsiderBuildSlow|4|Erstellen von Windows-Insider - langsam|
|windowsInsiderBuildRelease|5|Windows-Insider Build-Version|




