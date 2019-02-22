---
title: windowsUpdateStatus-Enumerationstyp
description: Windows Update for Business-Konfigurations Gerätestatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7549fb77cf5a9f7c3014192d5524019323405f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154159"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows Update for Business-Konfigurations Gerätestatus

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|upToDate|0|Es sind keine Updates, keine ausstehenden Neustart Updates und keine fehlerhaften Updates vorhanden.|
|pendingInstallation|1|Es gibt Updates für die Installation, die nicht genehmigte Updates enthalten. Es sind keine Updates für den Neustart vorhanden, keine fehlerhaften Aktualisierungen.|
|pendingReboot|2|Es gibt Updates, die einen Neustart erfordern. Es sind keine fehlerhaften Aktualisierungen vorhanden.|
|failed|3|Es sind keine Updates auf dem Gerät installiert.|




