---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065907"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>WindowsPrivacyDataAccessLevel Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Keine Zugriffsebene angegeben, keine Intents. Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten. Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.|
|forceAllow|1|Apps dürfen die angegebenen private Daten zugreifen.|
|forceDeny|2|Apps werden für den angegebenen Datenschutzinformationen Zugriff auf verweigert.|
|userInControl|3|Benutzer werden aufgefordert, wenn apps auf angegebenen Datenschutzinformationen zugreifen.|





