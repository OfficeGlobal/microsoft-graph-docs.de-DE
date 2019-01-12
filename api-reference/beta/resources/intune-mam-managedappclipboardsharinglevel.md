---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968416"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>ManagedAppClipboardSharingLevel Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|allApps|0|Freigabe zwischen alle apps, verwaltete oder nicht zulässig|
|managedAppsWithPasteIn|1|Freigabe ist zulässig zwischen alle verwalteten apps mit Einfügen in aktiviert|
|managedApps|2|Freigabe ist zwischen alle verwalteten apps zulässig.|
|gesperrt|3|Freigabe von zwischen apps ist deaktiviert.|





