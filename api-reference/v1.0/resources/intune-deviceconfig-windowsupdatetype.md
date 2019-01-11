---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838969"
---
# <a name="windowsupdatetype-enum-type"></a>WindowsUpdateType Enum-Typ

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



