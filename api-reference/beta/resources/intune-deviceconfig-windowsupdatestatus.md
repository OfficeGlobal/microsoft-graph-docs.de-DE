---
title: WindowsUpdateStatus Enum-Typ
description: Windows-update für Business Konfiguration Gerätestatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431564"
---
# <a name="windowsupdatestatus-enum-type"></a>WindowsUpdateStatus Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Windows-update für Business Konfiguration Gerätestatus

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Aktuellste|0|Es gibt keine ausstehende Updates, keine ausstehende Updates einen Neustart und keine fehlgeschlagenen Updates.|
|pendingInstallation|1|Es sind Updates, die die ausstehende Installation der Updates enthält, die nicht genehmigt werden. Es sind keine ausstehenden Neustarts Updates, keine fehlgeschlagenen Updates.|
|pendingReboot|2|Es sind Updates, die Neustart erforderlich ist. Es sind nicht fehlgeschlagenen Updates.|
|failed|3|Es sind Updates konnte nicht auf dem Gerät installiert werden.|




