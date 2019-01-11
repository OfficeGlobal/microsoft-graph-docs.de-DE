---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 477f0b52342ca1b27d844a5f03aedd806cdd8b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875831"
---
# <a name="safesearchfiltertype-enum-type"></a>SafeSearchFilterType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|Strict|1|Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.|
|Moderater|2|Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).|





