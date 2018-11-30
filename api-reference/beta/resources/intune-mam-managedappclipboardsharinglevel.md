---
title: ManagedAppClipboardSharingLevel Enum-Typ
description: Stellt die Ebene, zu der das Gerät Zwischenablage von apps gemeinsam verwendet wird
ms.openlocfilehash: 71c4ab2d629fdfee3ded68612d7060a0fa069809
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065610"
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





