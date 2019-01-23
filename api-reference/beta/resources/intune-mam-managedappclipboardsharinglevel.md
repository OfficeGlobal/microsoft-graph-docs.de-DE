---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410987"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>ManagedAppClipboardSharingLevel Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|allApps|0|Freigabe zwischen alle apps, verwaltete oder nicht zulässig|
|managedAppsWithPasteIn|1|Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert|
|managedApps|2|Freigabe ist zwischen alle verwalteten apps zulässig.|
|gesperrt|3|Freigabe von zwischen apps ist deaktiviert.|




