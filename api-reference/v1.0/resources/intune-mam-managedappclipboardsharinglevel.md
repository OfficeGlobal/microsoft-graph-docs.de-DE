---
title: managedAppClipboardSharingLevel-Enumerationstyp
description: Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250026"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt die Ebene dar, in der die Zwischenablage des Geräts zwischen apps freigegeben werden kann.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|allApps|0|Freigabe ist zwischen allen apps zulässig, verwaltet oder nicht|
|managedAppsWithPasteIn|1|Freigabe ist zwischen allen verwalteten apps zulässig, wobei Paste aktiviert ist.|
|managedApps|2|Freigabe ist zwischen allen verwalteten apps zulässig|
|gesperrt|3|Die Freigabe zwischen Apps ist deaktiviert|



