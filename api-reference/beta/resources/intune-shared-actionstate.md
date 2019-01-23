---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421613"
---
# <a name="actionstate-enum-type"></a>ActionState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Status der Aktion auf dem Gerät

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Nicht auf einen gültigen Action Zustand|
|Ausstehende|1|Aktion steht noch aus|
|abgebrochen|2|Aktion wurde abgebrochen.|
|aktive|3|Aktion ist aktiv.|
|done|4|Aktion ohne Fehler abgeschlossen.|
|failed|5|Aktion ist fehlgeschlagen|
|notSupported|6|Aktion wird nicht unterstützt.|




