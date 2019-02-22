---
title: edgeKioskModeRestrictionType-Enumerationstyp
description: Geben Sie an, wie die Microsoft-Edgeeinstellungen basierend auf dem Kioskmodus eingeschränkt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0dcd1d30895acbdecf9d9cc706ee14b7907f14f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177959"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Geben Sie an, wie die Microsoft-Edgeeinstellungen basierend auf dem Kioskmodus eingeschränkt werden.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Nicht konfiguriert (Unrestricted).|
|digitalSignage|1|Interaktive/digitale Beschilderung im Einzel-APP-Modus.|
|normalMode|2|Normaler Modus (Vollversion von Microsoft Edge).|
|publicBrowsingSingleApp|3|Öffentliches Browsen im Einzel-APP-Modus.|
|publicBrowsingMultiApp|4|Öffentliches Browsen (inPrivate) im Multi-APP-Modus.|




