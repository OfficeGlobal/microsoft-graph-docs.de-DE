---
title: BrowserSyncSetting Enum-Typ
description: Allow(Not Configured) oder prevent(Block) der Synchronisierung von Microsoft Edge Browsereinstellungen. Option, um zu verhindern, dass die Synchronisierung für Geräte, Benutzer außer Kraft setzen, aber zulassen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431500"
---
# <a name="browsersyncsetting-enum-type"></a>BrowserSyncSetting Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Allow(Not Configured) oder prevent(Block) der Synchronisierung von Microsoft Edge Browsereinstellungen. Option, um zu verhindern, dass die Synchronisierung für Geräte, Benutzer außer Kraft setzen, aber zulassen.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Standard – Synchronisierung von Browsereinstellungen für Geräte zulassen.|
|blockedWithUserOverride|1|Synchronisieren von Browsereinstellungen für Benutzer Geräte zu verhindern, Überschreiben der Einstellung Benutzer zulassen.|
|gesperrt|2|Absolut zu verhindern, dass die Synchronisierung von Browsereinstellungen für Benutzer Geräte.|




