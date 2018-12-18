---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
ms.openlocfilehash: eb0c7cfb862364ddc4703c89d19ea844ada6466d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343197"
---
# <a name="safesearchfiltertype-enum-type"></a>SafeSearchFilterType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|Strict|1|Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.|
|Moderater|2|Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).|



