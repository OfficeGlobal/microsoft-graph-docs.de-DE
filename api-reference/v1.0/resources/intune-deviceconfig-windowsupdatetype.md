---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
ms.openlocfilehash: 415dde619529ffa9bb40ab2cea36665558bb0ee9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340838"
---
# <a name="windowsupdatetype-enum-type"></a>WindowsUpdateType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Welche Geräte Branch erhält ihre Updates aus
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|all|1|Semikolons jährlichen Channel (Ziel). Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.|
|businessReadyOnly|2|Semikolons jährlichen Channel. Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.|
|windowsInsiderBuildFast|3|Erstellen von Windows-Insider - Fast|
|windowsInsiderBuildSlow|4|Erstellen von Windows-Insider - langsam|
|windowsInsiderBuildRelease|5|Windows-Insider Build-Version|



