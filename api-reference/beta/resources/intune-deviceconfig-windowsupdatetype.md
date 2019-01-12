---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1444af64043ac38685ca022b56b8856be77a0b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944348"
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





