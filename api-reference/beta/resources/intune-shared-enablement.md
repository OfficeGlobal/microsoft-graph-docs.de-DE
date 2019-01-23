---
title: Aktivierung von Steuerelementen Enum-Typ
description: Beschreibt die Aktivierung von Steuerelementen Enumeration die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399563"
---
# <a name="enablement-enum-type"></a>Aktivierung von Steuerelementen Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Werte verwendet, um den Status eines Geräts angeben. 

Beachten Sie, dass es ein Unterschied zwischen deaktiviert und nicht konfiguriert.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Gerät Standardwert, keine beabsichtigt.|
|enabled|1|Aktiviert die Einstellung auf dem Gerät.|
|deaktiviert|2|Deaktiviert die Einstellung auf dem Gerät.|
