---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888774"
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





