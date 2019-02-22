---
title: windowsPrivacyDataAccessLevel-Enumerationstyp
description: Bestimmen Sie die Zugriffsebene für bestimmte Windows-Datenschutzkategorien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2cdf124d3da6bf2c08954365a87ae0a97b05267
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159066"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Bestimmen Sie die Zugriffsebene für bestimmte Windows-Datenschutzkategorien.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Keine Zugriffsebene angegeben, keine Absichten. Das Gerät kann sich entweder wie in UserInControl oder in ForceAllow Verhalten. Es kann davon abhängen, auf welche Daten auf dem Datenschutz zugegriffen wurde, wie Windows-Versionen und andere Faktoren.|
|forceAllow|1|Apps können auf die angegebenen Datenschutz Daten zugreifen.|
|forceDeny|2|Apps wird der Zugriff auf die angegebenen Datenschutz Daten verweigert.|
|userInControl|3|Benutzer werden aufgefordert, wenn apps versuchen, auf die angegebenen Datenschutz Daten zuzugreifen.|




