---
title: MacOSGatekeeperAppSources Enum-Typ
description: App-Optionen für Mac OS Gatekeeper Quelle.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c2c1d553408b7269a53f9fc3500493a44bc3645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918114"
---
# <a name="macosgatekeeperappsources-enum-type"></a>MacOSGatekeeperAppSources Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

App-Optionen für Mac OS Gatekeeper Quelle.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Gerät Standardwert, keine beabsichtigt.|
|macAppStore|1|Nur apps aus der Mac-AppStore können ausgeführt werden.|
|macAppStoreAndIdentifiedDevelopers|2|Nur apps aus dem Mac AppStore und identifizierten Entwickler können ausgeführt werden.|
|an einer beliebigen Stelle|3|Apps unabhängig vom Standort können ausgeführt werden.|





